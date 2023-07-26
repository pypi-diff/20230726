# Comparing `tmp/hashwise-0.0.3.tar.gz` & `tmp/hashwise-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashwise-0.0.3.tar", last modified: Wed Jul 26 15:15:43 2023, max compression
+gzip compressed data, was "hashwise-0.0.4.tar", last modified: Wed Jul 26 15:29:45 2023, max compression
```

## Comparing `hashwise-0.0.3.tar` & `hashwise-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 15:15:43.355000 hashwise-0.0.3/
--rw-rw-rw-   0        0        0     3933 2023-07-26 15:15:43.347000 hashwise-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3713 2023-07-26 15:08:40.000000 hashwise-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 15:15:43.236000 hashwise-0.0.3/hashwise/
--rw-rw-rw-   0        0        0       23 2023-07-13 01:35:56.000000 hashwise-0.0.3/hashwise/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:15:43.317000 hashwise-0.0.3/hashwise/cuda-libraries/
--rw-rw-rw-   0        0        0   667648 2023-07-18 15:25:23.000000 hashwise-0.0.3/hashwise/cuda-libraries/cudalib-windows-64bit.dll
-drwxrwxrwx   0        0        0        0 2023-07-26 15:15:43.337000 hashwise-0.0.3/hashwise/device-info/
--rw-rw-rw-   0        0        0   257024 2023-07-16 00:54:58.000000 hashwise-0.0.3/hashwise/device-info/device-info.dll
--rw-rw-rw-   0        0        0     2648 2023-07-16 01:17:49.000000 hashwise-0.0.3/hashwise/device_status.py
--rw-rw-rw-   0        0        0      413 2023-07-17 02:24:41.000000 hashwise-0.0.3/hashwise/exceptions.py
--rw-rw-rw-   0        0        0    21646 2023-07-26 15:14:46.000000 hashwise-0.0.3/hashwise/hashwise.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:15:43.294000 hashwise-0.0.3/hashwise.egg-info/
--rw-rw-rw-   0        0        0     3933 2023-07-26 15:15:42.000000 hashwise-0.0.3/hashwise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-07-26 15:15:43.000000 hashwise-0.0.3/hashwise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 15:15:42.000000 hashwise-0.0.3/hashwise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-26 15:15:43.000000 hashwise-0.0.3/hashwise.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 15:15:43.000000 hashwise-0.0.3/hashwise.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 15:15:43.353000 hashwise-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      765 2023-07-26 15:14:43.000000 hashwise-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:29:45.506000 hashwise-0.0.4/
+-rw-rw-rw-   0        0        0     3933 2023-07-26 15:29:45.497000 hashwise-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3713 2023-07-26 15:08:40.000000 hashwise-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 15:29:45.392000 hashwise-0.0.4/hashwise/
+-rw-rw-rw-   0        0        0       23 2023-07-13 01:35:56.000000 hashwise-0.0.4/hashwise/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:29:45.471000 hashwise-0.0.4/hashwise/cuda-libraries/
+-rw-rw-rw-   0        0        0   667648 2023-07-18 15:25:23.000000 hashwise-0.0.4/hashwise/cuda-libraries/cudalib-windows-64bit.dll
+drwxrwxrwx   0        0        0        0 2023-07-26 15:29:45.487000 hashwise-0.0.4/hashwise/device-info/
+-rw-rw-rw-   0        0        0   257024 2023-07-16 00:54:58.000000 hashwise-0.0.4/hashwise/device-info/device-info.dll
+-rw-rw-rw-   0        0        0     2826 2023-07-26 15:27:55.000000 hashwise-0.0.4/hashwise/device_status.py
+-rw-rw-rw-   0        0        0      413 2023-07-17 02:24:41.000000 hashwise-0.0.4/hashwise/exceptions.py
+-rw-rw-rw-   0        0        0    21682 2023-07-26 15:28:48.000000 hashwise-0.0.4/hashwise/hashwise.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:29:45.450000 hashwise-0.0.4/hashwise.egg-info/
+-rw-rw-rw-   0        0        0     3933 2023-07-26 15:29:45.000000 hashwise-0.0.4/hashwise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-07-26 15:29:45.000000 hashwise-0.0.4/hashwise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 15:29:45.000000 hashwise-0.0.4/hashwise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-26 15:29:45.000000 hashwise-0.0.4/hashwise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 15:29:45.000000 hashwise-0.0.4/hashwise.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 15:29:45.504000 hashwise-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      765 2023-07-26 15:28:02.000000 hashwise-0.0.4/setup.py
```

### Comparing `hashwise-0.0.3/PKG-INFO` & `hashwise-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashwise
-Version: 0.0.3
+Version: 0.0.4
 Summary: A secure python library for GPU accelerated hashing.
 Author: Anish Kanthamneni
 Author-email: akneni@gmail.com
 Description-Content-Type: text/markdown
 
 # Hashwise Python Library
```

### Comparing `hashwise-0.0.3/README.md` & `hashwise-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hashwise-0.0.3/hashwise/cuda-libraries/cudalib-windows-64bit.dll` & `hashwise-0.0.4/hashwise/cuda-libraries/cudalib-windows-64bit.dll`

 * *Files identical despite different names*

### Comparing `hashwise-0.0.3/hashwise/device-info/device-info.dll` & `hashwise-0.0.4/hashwise/device-info/device-info.dll`

 * *Files identical despite different names*

### Comparing `hashwise-0.0.3/hashwise/device_status.py` & `hashwise-0.0.4/hashwise/device_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-import ctypes
+import ctypes as _ctypes
+import os as _os
+from pathlib import Path as _Path
 
 class DeviceStatus():
     __status = []
     __initialized = False
     __device_info_clib = None
 
     @classmethod
     def __init(cls):
-        cls.__initialized = True
-        cls.__device_info_clib = ctypes.cdll.LoadLibrary('./device-info/device-info.dll')
+        device_info_path = _Path(_os.path.dirname(_os.path.realpath(__file__))) / "device-info" / "device-info.dll"
+        cls.__device_info_clib = _ctypes.cdll.LoadLibrary(str(device_info_path))
 
-        cls.__device_info_clib.num_devices.restype = ctypes.c_int
-        cls.__device_info_clib.get_device_compute_capability.restype = ctypes.c_double
-        cls.__device_info_clib.get_device_name.restype = ctypes.c_char_p
-        cls.__device_info_clib.get_num_blocks.restype = ctypes.c_int
-        cls.__device_info_clib.get_max_threads_per_block.restype = ctypes.c_int
+        cls.__device_info_clib.num_devices.restype = _ctypes.c_int
+        cls.__device_info_clib.get_device_compute_capability.restype = _ctypes.c_double
+        cls.__device_info_clib.get_device_name.restype = _ctypes.c_char_p
+        cls.__device_info_clib.get_num_blocks.restype = _ctypes.c_int
+        cls.__device_info_clib.get_max_threads_per_block.restype = _ctypes.c_int
     
+        cls.__initialized = True
         if cls.__device_info_clib.num_devices() <= 0: return 
 
         cls.__status.append({
-            "name": ctypes.string_at(cls.__device_info_clib.get_device_name()).decode('utf-8'),
+            "name": _ctypes.string_at(cls.__device_info_clib.get_device_name()).decode('utf-8'),
             "compute_capability":cls.__device_info_clib.get_device_compute_capability(),
             'num_blocks':cls.__device_info_clib.get_num_blocks(),
             'threads_per_block':cls.__device_info_clib.get_max_threads_per_block(),
         })
 
     @classmethod
     def num_devices(cls):
```

### Comparing `hashwise-0.0.3/hashwise/hashwise.py` & `hashwise-0.0.4/hashwise/hashwise.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,15 @@
             for i in permutation_generator:
                 byte_obj = bytes(i)
                 if hash_algorithm(byte_obj) == target:
                     return i
             
     return None
 
-def brute_force_time_estimate(hash_algorithm, possible_elements, length:int=None, string_encoding:str='utf-8', units='seconds', num_trials=None):
+def brute_force_time_estimate(hash_algorithm, possible_elements, len_permutation:int=None, string_encoding:str='utf-8', units='seconds', num_trials=None):
     """
     This function estimates the time it would take to brute force a hashed string using a specified hash algorithm and possible elements.
 
     Parameters:
     hash_algorithm: A hashing algorithm from the hashwise library.
     possible_elements: A string or collection of characters to be used for generating permutations, or a range object or list/tuple specifying a range of integers.
     length (int, optional): The length of the permutations to be generated. Required if possible_elements is a collection of characters.
@@ -398,17 +398,17 @@
     units = units.lower()
     if units not in unit_lst['units']:
         raise ValueError ("Argument 'units' must one of", unit_lst["units"])
 
     # checks and formats the possible_elements argument
     gen_type = str
     if isinstance(possible_elements, str) or all([isinstance(i, str) for i in possible_elements]):
-        permutation_generator = __perm_gen_str(possible_elements, length)
-        permutation_length = len(possible_elements)**length
-        if length is None:
+        permutation_generator = __perm_gen_str(possible_elements, len_permutation)
+        permutation_length = len(possible_elements)**len_permutation
+        if len_permutation is None:
             raise TypeError("Argument 'length' must be defined when lassing colections of chars to 'possible_elements'")
     elif 1 <= len(possible_elements) <= 3 and all([isinstance(i, (int)) for i in possible_elements]):
         if len(possible_elements) == 1:
             possible_elements = [0, possible_elements[0], 1]
         elif len(possible_elements) == 2:
             possible_elements = [possible_elements[0], possible_elements[1], 1]
         permutation_generator = __perm_gen_num(*possible_elements)
```

### Comparing `hashwise-0.0.3/hashwise.egg-info/PKG-INFO` & `hashwise-0.0.4/hashwise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashwise
-Version: 0.0.3
+Version: 0.0.4
 Summary: A secure python library for GPU accelerated hashing.
 Author: Anish Kanthamneni
 Author-email: akneni@gmail.com
 Description-Content-Type: text/markdown
 
 # Hashwise Python Library
```

### Comparing `hashwise-0.0.3/setup.py` & `hashwise-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='hashwise',
-    version='0.0.3',
+    version='0.0.4',
     description='A secure python library for GPU accelerated hashing.',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     author='Anish Kanthamneni',
     packages=find_packages(),
     package_data={
         '': ['*.dll'],
```

