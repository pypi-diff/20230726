# Comparing `tmp/tritondse-0.1.5.tar.gz` & `tmp/tritondse-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritondse-0.1.5.tar", last modified: Thu Jul 20 12:42:02 2023, max compression
+gzip compressed data, was "tritondse-0.1.6.tar", last modified: Wed Jul 26 09:32:36 2023, max compression
```

## Comparing `tritondse-0.1.5.tar` & `tritondse-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:02.297245 tritondse-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 12:41:58.000000 tritondse-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-20 12:42:02.297245 tritondse-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-20 12:41:58.000000 tritondse-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:42:02.297245 tritondse-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-20 12:41:58.000000 tritondse-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:02.297245 tritondse-0.1.5/tritondse/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    36167 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29681 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/heap_allocator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:02.297245 tritondse-0.1.5/tritondse/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/loaders/cle_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/loaders/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/loaders/quokkaprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:02.297245 tritondse-0.1.5/tritondse/probes/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/probes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/probes/basic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    50989 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/process_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/qbdi_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    75406 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/sanitizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/seeds_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    35983 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/symbolic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/symbolic_explorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/thread_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/worklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-20 12:41:58.000000 tritondse-0.1.5/tritondse/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:42:02.297245 tritondse-0.1.5/tritondse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-20 12:42:02.000000 tritondse-0.1.5/tritondse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-20 12:42:02.000000 tritondse-0.1.5/tritondse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:42:02.000000 tritondse-0.1.5/tritondse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 12:42:02.000000 tritondse-0.1.5/tritondse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 12:42:02.000000 tritondse-0.1.5/tritondse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:36.062479 tritondse-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 09:32:34.000000 tritondse-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-26 09:32:36.062479 tritondse-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-26 09:32:34.000000 tritondse-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:32:36.062479 tritondse-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-26 09:32:34.000000 tritondse-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:36.062479 tritondse-0.1.6/tritondse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36167 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29299 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/heap_allocator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:36.062479 tritondse-0.1.6/tritondse/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/loaders/cle_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/loaders/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/loaders/quokkaprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22834 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:36.062479 tritondse-0.1.6/tritondse/probes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/probes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/probes/basic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52218 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/process_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/qbdi_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75406 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/sanitizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/seeds_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36666 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/symbolic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/symbolic_explorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/thread_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/worklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-07-26 09:32:34.000000 tritondse-0.1.6/tritondse/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:32:36.062479 tritondse-0.1.6/tritondse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-26 09:32:36.000000 tritondse-0.1.6/tritondse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 09:32:36.000000 tritondse-0.1.6/tritondse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:32:36.000000 tritondse-0.1.6/tritondse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 09:32:36.000000 tritondse-0.1.6/tritondse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 09:32:36.000000 tritondse-0.1.6/tritondse.egg-info/top_level.txt
```

### Comparing `tritondse-0.1.5/LICENSE` & `tritondse-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/PKG-INFO` & `tritondse-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.5 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.6 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.5/README.md` & `tritondse-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/setup.py` & `tritondse-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md") as f:
     README = f.read()
 
 
 setup(
     name="tritondse",
-    version="0.1.5",
+    version="0.1.6",
     description="A library of Dynamic Symbolic Exploration based the Triton library",
     packages=find_packages(),
     long_description=README,
     long_description_content_type='text/markdown',
     url="https://github.com/quarkslab/tritondse",
     project_urls={
         "Documentation": "https://quarkslab.github.io/tritondse/",
```

### Comparing `tritondse-0.1.5/tritondse/__init__.py` & `tritondse-0.1.6/tritondse/__init__.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/arch.py` & `tritondse-0.1.6/tritondse/arch.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/callbacks.py` & `tritondse-0.1.6/tritondse/callbacks.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/config.py` & `tritondse-0.1.6/tritondse/config.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/coverage.py` & `tritondse-0.1.6/tritondse/coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,25 +509,14 @@
                     else:
                         self._not_covered_items_mirror[edge].append(prefix)
 
         else: # Straightfoward set difference
             self.not_covered_items.update(other.not_covered_items - self.covered_items.keys())
 
 
-    def improves_coverage(self, other: CoverageSingleRun) -> bool:
-        """
-        Check if `other` improves coverage
-        Used to know if an input is relevant to keep or not
-
-        :param other: The CoverageSingleRun to check against our global coverage state
-        :return: bool
-        """
-        return bool(other.covered_items.keys() - self.covered_items.keys())
-
-
     def can_improve_coverage(self, other: CoverageSingleRun) -> bool:
         """
         Check if some of the non-covered are not already in the global coverage
         Used to know if an input is relevant to keep or not
 
         :param other: The CoverageSingleRun to check against our global coverage state
         :return: bool
```

### Comparing `tritondse-0.1.5/tritondse/exception.py` & `tritondse-0.1.6/tritondse/exception.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/heap_allocator.py` & `tritondse-0.1.6/tritondse/heap_allocator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/loaders/cle_loader.py` & `tritondse-0.1.6/tritondse/loaders/cle_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 
 # Third-party imports
 import cle
 
 # Local imports
 from tritondse.loaders import Loader, LoadableSegment
-from tritondse.types import Addr, Architecture, PathLike, Platform, Perm
+from tritondse.types import Addr, Architecture, PathLike, Platform, Perm, Endian
 from tritondse.routines import SUPPORTED_ROUTINES
 import tritondse.logging
 
 logger = tritondse.logging.get("loader")
 
 _arch_mapper = {
     "ARMEL":   Architecture.ARM32,
@@ -61,14 +61,19 @@
         Architecture enum representing program architecture.
 
         :rtype: Architecture
         """
         return _arch_mapper[self.ld.main_object.arch.name]
 
     @property
+    def endianness(self) -> Endian:
+        # FIXME: Depending on architecture returning good endianess
+        return Endian.LITTLE
+
+    @property
     def entry_point(self) -> Addr:
         """
         Program entrypoint address as defined in the binary headers
 
         :rtype: :py:obj:`tritondse.types.Addr`
         """
         return self.ld.main_object.entry
```

### Comparing `tritondse-0.1.5/tritondse/loaders/loader.py` & `tritondse-0.1.6/tritondse/loaders/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 # built-in imports
-from collections import namedtuple
 from pathlib import Path
-from typing import Optional, Generator, Tuple, Dict, Union, List
+from typing import Optional, Generator, Tuple, Dict, List
 from dataclasses import dataclass
 
 # local imports
-from tritondse.types import Addr, Architecture, Platform, ArchMode, PathLike, Perm
+from tritondse.types import Addr, Architecture, Platform, ArchMode, Perm, Endian
 from tritondse.arch import ARCHS
 import tritondse.logging
 
 logger = tritondse.logging.get()
 
 
 @dataclass
@@ -81,14 +80,23 @@
         """
         Platform of the binary.
 
         :return: Platform
         """
         return None
 
+    @property
+    def endianness(self) -> Endian:
+        """
+        Endianess of the loaded program
+
+        :return: Endianness
+        """
+        raise NotImplementedError()
+
     def memory_segments(self) -> Generator[LoadableSegment, None, None]:
         """
         Iterate over all memory segments of the program as loaded in memory.
 
         :return: Generator of tuples addrs and content
         :raise NotImplementedError: if the binary format cannot be loaded
         """
@@ -140,22 +148,24 @@
     """
 
     def __init__(self,
                  architecture: Architecture,
                  cpustate: Dict[str, int] = None,
                  maps: List[LoadableSegment] = None,
                  set_thumb: bool = False,
-                 platform: Platform = None):
+                 platform: Platform = None,
+                 endianess: Endian = Endian.LITTLE):
         super(MonolithicLoader, self).__init__("")
 
         self._architecture = architecture
         self._platform = platform if platform else None
         self._cpustate = cpustate if cpustate else {}
         self.maps = maps
         self._arch_mode = ArchMode.THUMB if set_thumb else None
+        self._endian = endianess
         if self._platform and (self._architecture, self._platform) in ARCHS:
             self._archinfo = ARCHS[(self._architecture, self._platform)]
         elif self._architecture in ARCHS:
             self._archinfo = ARCHS[self._architecture]
         else: 
             logger.error("Unknown architecture")
             assert False
@@ -213,7 +223,15 @@
     def platform(self) -> Optional[Platform]:
         """
         Platform of the binary.
 
         :return: Platform
         """
         return self._platform
+
+    @property
+    def endianness(self) -> Endian:
+        """
+        Endianess of the monolithic loader.
+        (default is LITTLE)
+        """
+        return self._endian
```

### Comparing `tritondse-0.1.5/tritondse/loaders/program.py` & `tritondse-0.1.6/tritondse/loaders/program.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,17 +71,18 @@
         self._funs = {f.name: f for f in self._binary.concrete.functions}
 
     @property
     def name(self) -> str:
         """ Name of the loader"""
         return f"Program({self.path})"
 
-    def endianess(self) -> Endian:
-        # FIXME: Depending on architecture returning good endianess
-        return Endian.LITTLE
+    @property
+    def endianness(self) -> Endian:
+        return {lief.ENDIANNESS.LITTLE: Endian.LITTLE,
+                lief.ENDIANNESS.BIG: Endian.BIG}[self._binary.abstract.header.endianness]
 
     @property
     def entry_point(self) -> Addr:
         """
         Program entrypoint address as defined in the binary headers
 
         :rtype: :py:obj:`tritondse.types.Addr`
@@ -104,23 +105,14 @@
         of the file ELF, PE etc..
 
         :return: Platform
         """
         return self._plfm
 
     @property
-    def endianness(self) -> lief.ENDIANNESS:
-        """
-        Endianness of the program as defined in binary headers.
-
-        :rtype: lief.ENDIANNESS
-        """
-        return self._binary.abstract.header.endianness
-
-    @property
     def format(self) -> lief.EXE_FORMATS:
         """
         Binary format. Supported formats by lief are: ELF, PE, MachO
 
         :rtype: lief.EXE_FORMATS
         """
         return self._binary.format
```

### Comparing `tritondse-0.1.5/tritondse/loaders/quokkaprogram.py` & `tritondse-0.1.6/tritondse/loaders/quokkaprogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import quokka
 import networkx
 import lief
 
 # local imports
 from tritondse.loaders import Program, LoadableSegment
 from tritondse.coverage import CoverageSingleRun
-from tritondse.types import PathLike, Addr, Architecture, Platform
+from tritondse.types import PathLike, Addr, Architecture, Platform, Endian
 
 
 class QuokkaProgram(quokka.Program):
     def __init__(self, export_file: Union[Path, str], exec_path: Union[Path, str]):
         super(QuokkaProgram, self).__init__(export_file, exec_path)
 
         self.program = Program(self.executable.exec_file.as_posix())
@@ -93,15 +93,15 @@
         return self.program.architecture
 
     @property
     def platform(self) -> Platform:
         return self.program.platform
 
     @property
-    def endianness(self) -> lief.ENDIANNESS:
+    def endianness(self) -> Endian:
         return self.program.endianness
 
     @property
     def format(self) -> lief.EXE_FORMATS:
         return self.program.format
 
     @property
```

### Comparing `tritondse-0.1.5/tritondse/logging.py` & `tritondse-0.1.6/tritondse/logging.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/memory.py` & `tritondse-0.1.6/tritondse/memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,24 +84,24 @@
     Memory representation of the current :py:class:`ProcessState` object.
     It wraps all interaction with Triton's memory context to provide high-level
     function. It adds a segmentation and memory permission model at the top
     of Triton. It also overrides __getitem__ and the slice mechanism to be able
     read and write concrete memory values in a Pythonic manner.
     """
 
-    def __init__(self, ctx: TritonContext):
+    def __init__(self, ctx: TritonContext, endianness: Endian = Endian.LITTLE):
         """
         :param ctx: TritonContext to interface with
         """
         self.ctx: TritonContext = ctx
         """Underlying Triton context"""
         self._linear_map_addr = []  # List of [map_start, map_end, map_start, map_end ...]
         self._linear_map_map = []   # List of [MemMap,    None,    MemMap,    None    ...]
         self._segment_enabled = True
-        self._endian = Endian.LITTLE
+        self._endian = endianness
         self._endian_key = ENDIAN_MAP[self._endian]
         self._mem_cbs_enabled = True
         # self._maps = {}  # Addr: -> Map
 
     def set_endianess(self, en: Endian) -> None:
         """
         Set the endianness of memory accesses. By default,
```

### Comparing `tritondse-0.1.5/tritondse/probes/basic_trace.py` & `tritondse-0.1.6/tritondse/probes/basic_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/process_state.py` & `tritondse-0.1.6/tritondse/process_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # built-ins
 from __future__ import annotations
 
 import io
+import struct
 import sys
 import time
 from typing import Union, Callable, Tuple, Optional, List, Dict
 
 
 # third-party
 # import z3  # For direct value enumeration
 from triton import TritonContext, MemoryAccess, CALLBACK, CPUSIZE, Instruction, MODE, AST_NODE, SOLVER, EXCEPTION
 
 # local imports
 from tritondse.thread_context import ThreadContext
 from tritondse.heap_allocator import HeapAllocator
 from tritondse.types import Architecture, Addr, ByteSize, BitSize, PathConstraint, Register, Expression, \
-                            AstNode, Registers, SolverStatus, Model, SymbolicVariable, ArchMode, Perm, FileDesc
+                            AstNode, Registers, SolverStatus, Model, SymbolicVariable, ArchMode, Perm, FileDesc, Endian
 from tritondse.arch import ARCHS, CpuState
 from tritondse.loaders import Loader
 from tritondse.memory import Memory, MemoryAccessViolation
 import tritondse.logging
 
 logger = tritondse.logging.get()
 
@@ -32,17 +33,19 @@
     it provides a user-friendly API to access data in both the concrete and symbolic
     state of Triton.
     """
 
     STACK_SEG = "[stack]"
     EXTERN_SEG = "[extern]"
 
-    def __init__(self, time_inc_coefficient: float = 0.0001):
+    def __init__(self, endianness: Endian = Endian.LITTLE, time_inc_coefficient: float = 0.0001):
         """
-        :param time_inc_coefficient: Time coefficient to represent execution time of an instruction see: :py:attr:`tritondse.Config.time_inc_coefficient`
+        :param endianness: Endianness to consider
+        :param time_inc_coefficient: Time coefficient to represent execution time of an
+                                     instruction see: :py:attr:`tritondse.Config.time_inc_coefficient`
         """
         # EXTERN_BASE is a "fake" memory area (not mapped) that will
         # which addresses will be used for external symbols
         self.EXTERN_FUNC_BASE = 0x01000000  # Not PLT but a dummy address space containing pointers to external symbols
 
         # This range will be dynamically allocated
         # upon request.
@@ -59,15 +62,15 @@
         """
 
         # Cpu object wrapping registers values
         self.cpu: CpuState = None  #: CpuState holding concrete values of registers *(initialized when calling load)*
         self._archinfo = None
 
         # Memory object
-        self.memory: Memory = Memory(self.tt_ctx)
+        self.memory: Memory = Memory(self.tt_ctx, endianness)
         """Memory object associated with the ProcessState """
 
         # Used to define that the process must exist
         self.stop = False
 
         # Signals table used by raise(), signal(), etc.
         #self.signals_table = dict()
@@ -109,14 +112,15 @@
 
         # The time when the ProcessState is instancied.
         # It's used to provide a deterministic behavior when calling functions
         # like gettimeofday(), clock_gettime(), etc.
         self.time = time.time()
 
         # Configuration values
+        self.endianness = endianness  #: Current endianness
         self.time_inc_coefficient = time_inc_coefficient
 
         # Runtime temporary variables
         self.__pcs_updated = False
 
         # The current instruction executed
         self.__current_inst = None
@@ -409,14 +413,42 @@
         :type arch: Architecture
         :return: None
         """
         self.architecture = arch
         self._archinfo = ARCHS[self.architecture]
         self.cpu = CpuState(self.tt_ctx, self._archinfo)
 
+    def unpack_integer(self, data: bytes, size: int) -> int:
+        """
+        Unpack the given bytes into into integer value respecting
+        size given and endianness.
+
+        :param data: bytes data to unpack
+        :param size: size in bits of data to unpack
+        :return: integer value unpacked
+        """
+        s = "<" if self.endianness == Endian.LITTLE else ">"
+        tab = {8: 'B', 16: 'H', 32: 'I', 64: 'Q'}
+        s += tab[size]
+        return struct.unpack(s, data)[0]
+
+    def pack_integer(self, value: int, size: int) -> bytes:
+        """
+        Unpack the given bytes into into integer value respecting
+        size given and endianness.
+
+        :param data: bytes data to unpack
+        :param size: size in bits of data to unpack
+        :return: integer value packed as bytes
+        """
+        s = "<" if self.endianness == Endian.LITTLE else ">"
+        tab = {8: 'B', 16: 'H', 32: 'I', 64: 'Q'}
+        s += tab[size]
+        return struct.pack(s, value)
+
     def read_register(self, register: Union[str, Register]) -> int:
         """
         Read the current concrete value of the given register.
 
         :param register: string of the register or Register object
         :type register: Union[str, :py:obj:`tritondse.types.Register`]
         :return: Integer value
@@ -1133,15 +1165,15 @@
             else:
                 return result
             limit -= 1
         return result
 
     @staticmethod
     def from_loader(loader: Loader) -> 'ProcessState':
-        pstate = ProcessState()
+        pstate = ProcessState(loader.endianness)
 
         # Initialize the architecture of the processstate
         pstate.initialize_context(loader.architecture)
 
         # Set the program counter to points to entrypoint
         pstate.cpu.program_counter = loader.entry_point
 
@@ -1176,15 +1208,14 @@
 
                 else:
                     # Add symbol in dynamic_symbol_table
                     pstate.dynamic_symbol_table[fname] = (cur_linkage_address, True)
 
                     # Apply relocation to our custom address in process memory
                     pstate.memory.write_ptr(rel_addr, cur_linkage_address)
-
                     # Increment linkage address number
                     cur_linkage_address += pstate.ptr_size
 
         # Try initializing stack registers if a stack is present in maps
         # Map the stack
         try:
             stack = pstate.memory.map_from_name(pstate.STACK_SEG)
```

### Comparing `tritondse-0.1.5/tritondse/qbdi_trace.py` & `tritondse-0.1.6/tritondse/qbdi_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/routines.py` & `tritondse-0.1.6/tritondse/routines.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/sanitizers.py` & `tritondse-0.1.6/tritondse/sanitizers.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/seed.py` & `tritondse-0.1.6/tritondse/seed.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/seeds_manager.py` & `tritondse-0.1.6/tritondse/seeds_manager.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/symbolic_executor.py` & `tritondse-0.1.6/tritondse/symbolic_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     def _init_symbolic_seed(self, seed: Seed) -> Union[list, CompositeData]:
         if seed.is_raw():
             return [None]*len(seed.content)
         else:  # is composite
             argv = [[None]*len(a) for a in seed.content.argv]
             files = {k: [None]*len(v) for k, v in seed.content.files.items()}
-            variables = {k: [None]*len(v) for k, v in seed.content.variables.items()}
+            variables = {k: [None]*(1 if isinstance(v, int) else len(v)) for k, v in seed.content.variables.items()}
             return CompositeData(argv=argv, files=files, variables=variables)
 
     def load(self, loader: Loader) -> None:
         """
         Use the given loader to initialize the ProcessState.
         It overrides the current ProcessState if any.
 
@@ -681,21 +681,30 @@
 
             # Handle argv (its meant to be here)
             args = [bytearray(x) for x in self.seed.content.argv]
             new_argv = [bytes(repl_bytearray(c, s)) for c, s in zip(args, self._symbolic_seed.argv)]
 
             # Handle stdin and files
             # If the seed provides the content of files (#NOTE stdin is treated as a file)
-            new_files = {k: bytes(repl_bytearray(bytearray(c), self._symbolic_seed.files[k])) for k, c in
-                         self.seed.content.files.items() if k in self._symbolic_seed.files}
+            new_files = {}
+            for k, c in self.seed.content.files.items():
+                if k in self._symbolic_seed.files:
+                    new_files[k] = bytes(repl_bytearray(bytearray(c), self._symbolic_seed.files[k]))
+                else:
+                    new_files[k] = c  # keep the current value in the seed
 
-            # Handle variables
-            # If the seed provides the content of variables
-            new_variables = {k: bytes(repl_bytearray(bytearray(c), self._symbolic_seed.variables[k])) for k, c in
-                             self.seed.content.variables.items() if k in self._symbolic_seed.variables}
+            # Handle variables, if the seed provides some
+            new_variables = {}
+            for k, c in self.seed.content.variables.items():
+                if k in self._symbolic_seed.variables:
+                    conc = bytearray(c) if isinstance(c, bytes) else [c]
+                    new_vals = repl_bytearray(conc, self._symbolic_seed.variables[k])
+                    new_variables[k] = bytes(new_vals) if isinstance(c, bytes) else new_vals[0]  # new variables are either bytes or int
+                else:
+                    new_variables[k] = c  # If it has not been injected keep the current concrete value
 
             content = CompositeData(new_argv, new_files, new_variables)
         else:
             assert False
 
         # Calling callback if user defined one
         new_seed = Seed(content)
@@ -764,28 +773,33 @@
             logger.error("can't call inject_symbolic_file_register with regsiter larger than 1!")
             return
         self.pstate.write_register(reg, value)  # Write concrete value in register
         sym_vars = self.pstate.symbolize_register(reg, f"{name}[{offset}]")  # Symbolize bytes
         sym_seed = self._symbolic_seed.files[name] if self.seed.is_composite() else self._symbolic_seed
         sym_seed[offset] = sym_vars  # Add symbolic variables to symbolic seed
 
-    def inject_symbolic_variable_register(self, reg: Union[str, Register], name: str, value: int, offset: int = 0) -> None:
+    def inject_symbolic_variable_register(self, reg: Union[str, Register], name: str, value: int) -> None:
         """
         Inject a symbolic variable (or part of it) in a register.
         The value has to be an integer.
 
         :param reg: register identifier
         :param name: name of the variable
         :param value: integer value
-        :param offset: offset within the variable
         """
-        self.pstate.write_register(reg, value)  # Write concrete value in register
-        sym_vars = [self.pstate.symbolize_register(reg, f"{name}[{offset}]")] # Symbolize bytes
-        sym_seed = self._symbolic_seed.variables[name] if self.seed.is_composite() else self._symbolic_seed
-        sym_seed[offset] = sym_vars # Add symbolic variables to symbolic seed
+        if not self.seed.is_composite():
+            logger.warning("cannot use inject_symbolic_variable_register on raw seeds!")
+            return
+
+        if isinstance(value, int):
+            self.pstate.write_register(reg, value)                         # write concrete value in register
+            sym_var = self.pstate.symbolize_register(reg, f"{name}[{0}]")  # symbolize value
+            self._symbolic_seed.variables[name][0] = sym_var               # add the symbolic variables to symbolic seed
+        else:  # meant to be bytes
+            logger.warning("variable injected in registers have to be integer values")
 
     def inject_symbolic_raw_input(self, addr: Addr, data: bytes, offset: int = 0) -> None:
         """
         Inject the input in memory. This injection method should
         be used for RAW seed type.
 
         :param addr: address where to inject input.
```

### Comparing `tritondse-0.1.5/tritondse/symbolic_explorator.py` & `tritondse-0.1.6/tritondse/symbolic_explorator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/thread_context.py` & `tritondse-0.1.6/tritondse/thread_context.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/trace.py` & `tritondse-0.1.6/tritondse/trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/types.py` & `tritondse-0.1.6/tritondse/types.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/worklist.py` & `tritondse-0.1.6/tritondse/worklist.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse/workspace.py` & `tritondse-0.1.6/tritondse/workspace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.5/tritondse.egg-info/PKG-INFO` & `tritondse-0.1.6/tritondse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.5 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.6 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.5/tritondse.egg-info/SOURCES.txt` & `tritondse-0.1.6/tritondse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

