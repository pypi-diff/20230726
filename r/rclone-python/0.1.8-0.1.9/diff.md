# Comparing `tmp/rclone-python-0.1.8.tar.gz` & `tmp/rclone-python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclone-python-0.1.8.tar", last modified: Wed Jul 19 05:54:43 2023, max compression
+gzip compressed data, was "rclone-python-0.1.9.tar", last modified: Wed Jul 26 15:42:30 2023, max compression
```

## Comparing `rclone-python-0.1.8.tar` & `rclone-python-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:54:43.910553 rclone-python-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-19 05:54:32.000000 rclone-python-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-19 05:54:43.910553 rclone-python-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-19 05:54:32.000000 rclone-python-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:54:43.910553 rclone-python-0.1.8/rclone_python/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 05:54:32.000000 rclone-python-0.1.8/rclone_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-19 05:54:32.000000 rclone-python-0.1.8/rclone_python/extract_remotenames.py
--rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-07-19 05:54:32.000000 rclone-python-0.1.8/rclone_python/rclone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-19 05:54:32.000000 rclone-python-0.1.8/rclone_python/remote_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-19 05:54:32.000000 rclone-python-0.1.8/rclone_python/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:54:43.910553 rclone-python-0.1.8/rclone_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-19 05:54:43.000000 rclone-python-0.1.8/rclone_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-19 05:54:43.000000 rclone-python-0.1.8/rclone_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:54:43.000000 rclone-python-0.1.8/rclone_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 05:54:43.000000 rclone-python-0.1.8/rclone_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 05:54:43.000000 rclone-python-0.1.8/rclone_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:54:43.910553 rclone-python-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-19 05:54:32.000000 rclone-python-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:42:30.043859 rclone-python-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-26 15:42:20.000000 rclone-python-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-26 15:42:30.043859 rclone-python-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-26 15:42:20.000000 rclone-python-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:42:30.043859 rclone-python-0.1.9/rclone_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 15:42:20.000000 rclone-python-0.1.9/rclone_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-26 15:42:20.000000 rclone-python-0.1.9/rclone_python/hash_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-07-26 15:42:20.000000 rclone-python-0.1.9/rclone_python/rclone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-26 15:42:20.000000 rclone-python-0.1.9/rclone_python/remote_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-26 15:42:20.000000 rclone-python-0.1.9/rclone_python/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:42:30.043859 rclone-python-0.1.9/rclone_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-26 15:42:30.000000 rclone-python-0.1.9/rclone_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-26 15:42:30.000000 rclone-python-0.1.9/rclone_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:42:30.000000 rclone-python-0.1.9/rclone_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 15:42:30.000000 rclone-python-0.1.9/rclone_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 15:42:30.000000 rclone-python-0.1.9/rclone_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:42:30.043859 rclone-python-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-26 15:42:20.000000 rclone-python-0.1.9/setup.py
```

### Comparing `rclone-python-0.1.8/LICENSE` & `rclone-python-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.8/PKG-INFO` & `rclone-python-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,16 +24,19 @@
 
 ## Features ⚒️
 
 - Copy, move and sync files between remotes
 - Delete and prune files/directories
 - List files in a directory including properties of the files.
 - List available remotes.
+- Generate hashes from files or validate them with their hashsum.
 - Create new remotes
 - Check available remotes
+- Create and manage public links.
+- Check the currently installed rclone versions and if updates are available.
 
 ## Installation 💾
 
 _rclone_python_ can be installed using pip
 
 ```shell
 pip install rclone-python
@@ -106,7 +109,15 @@
 ```python
 from rclone_python import rclone
 
 # remove the entire test_dir folder (and all files contained in it and it's subdirectories) on onedrive
 rclone.purge('onedrive:test_dir')
 ```
 
+### Get Hash
+```python
+from rclone_python import rclone
+from rclone_python.hash_types import HashTypes
+
+print(rclone.hash(HashTypes.sha1, "box:data")
+# {'video1.webm': '3ef08d895f25e8b7d84d3a1ac58f8f302e33058b', 'video3.webm': '3ef08d895f25e8b7d84d3a1ac58f8f302e33058b', 'video2.webm': '3ef08d895f25e8b7d84d3a1ac58f8f302e33058b'}
+```
```

### Comparing `rclone-python-0.1.8/README.md` & `rclone-python-0.1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 
 ## Features ⚒️
 
 - Copy, move and sync files between remotes
 - Delete and prune files/directories
 - List files in a directory including properties of the files.
 - List available remotes.
+- Generate hashes from files or validate them with their hashsum.
 - Create new remotes
 - Check available remotes
+- Create and manage public links.
+- Check the currently installed rclone versions and if updates are available.
 
 ## Installation 💾
 
 _rclone_python_ can be installed using pip
 
 ```shell
 pip install rclone-python
@@ -92,7 +95,15 @@
 ```python
 from rclone_python import rclone
 
 # remove the entire test_dir folder (and all files contained in it and it's subdirectories) on onedrive
 rclone.purge('onedrive:test_dir')
 ```
 
+### Get Hash
+```python
+from rclone_python import rclone
+from rclone_python.hash_types import HashTypes
+
+print(rclone.hash(HashTypes.sha1, "box:data")
+# {'video1.webm': '3ef08d895f25e8b7d84d3a1ac58f8f302e33058b', 'video3.webm': '3ef08d895f25e8b7d84d3a1ac58f8f302e33058b', 'video2.webm': '3ef08d895f25e8b7d84d3a1ac58f8f302e33058b'}
+```
```

### Comparing `rclone-python-0.1.8/rclone_python/rclone.py` & `rclone-python-0.1.9/rclone_python/rclone.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
+import re
 import logging
 from functools import wraps
 from shutil import which
-from typing import Union, List, Dict, Callable, Any
+from typing import Optional, Union, List, Dict, Callable
 
 from rclone_python import utils
+from rclone_python.hash_types import HashTypes
 from rclone_python.remote_types import RemoteTypes
 
 
 def __check_installed(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         if not is_installed():
@@ -258,14 +260,15 @@
     if process.returncode == 0:
         logging.info(f"Successfully deleted {path}")
     else:
         raise Exception(
             f'Deleting path "{path}" failed with error message:\n{process.stderr}'
         )
 
+
 @__check_installed
 def link(
     path: str,
     expire: Union[str, None] = None,
     unlink=False,
     args=None,
 ) -> str:
@@ -328,26 +331,26 @@
         args.append("--files-only")
 
     process = utils.run_cmd(command, args)
 
     if process.returncode == 0:
         return json.loads(process.stdout)
     else:
-        raise Exception(f"ls operation on {path} failed with {process.stderr}")
+        raise Exception(f"ls operation on {path} failed with:\n{process.stderr}")
 
 
 def tree(
     path: str,
     args: List[str] = None,
 ) -> str:
     """Returns the contents of the remote path in a tree like fashion.
 
     Args:
         path (str): The path from which the tree should be generated
-        args (List[str], optional): Optional additional list of flags (e.g. ['--all', '--modtime']).
+        args (List[str], optional): Optional additional list of flags.
 
     Returns:
         str: String containing the file tree.
     """
     if args is None:
         args = []
 
@@ -356,14 +359,141 @@
     if process.returncode != 0:
         raise Exception(process.stderr)
     else:
         return process.stdout
 
 
 @__check_installed
+def hash(
+    hash: Union[str, HashTypes],
+    path: str,
+    download=False,
+    checkfile: Optional[str] = None,
+    output_file: Optional[str] = None,
+    args: List[str] = None,
+) -> Union[None, str, bool, Dict[str, str], Dict[str, bool]]:
+    """Produces a hashsum file for all the objects in the path.
+
+    Args:
+        hash (Union[str, HashTypes]): The hash algorithm to use, e.g. sha1. Depends on the backend used.
+        path (str): The path to the file/ folder to generate hashes for.
+        download (bool, optional): Download the file and hash it locally. Useful when the backend does not support the selected hash algorithm.
+        checkfile (Optional[str], optional):  Validate hashes against a given SUM file instead of printing them.
+        output_file (Optional[str], optional): Output hashsums to a file rather than the terminal (same format as the checkfile).
+        args (List[str], optional): Optional additional list of flags.
+
+    Raises:
+        Exception: Raised when the rclone command does not succeed.
+
+    Returns:
+        Union[None, str, bool, Dict[str, str], Dict[str, bool]]: 3 different modes apply based on the inputs:
+            1)  Nothing is returned when output file is set.
+            2)  When checkfile is set, a dictionary is returned with file names as keys.
+                The values are either True or False, depending on wether the file is valid ot not.
+                In the special case of only a single file, True or False is directly returned.
+            3)  If neither checkfile nor output_file is set, a dictionary is returned with file names as keys.
+                The values are the individual hash sums.
+                In the special case of only a single file, the hashsum is directly returned.
+    """
+
+    if isinstance(hash, HashTypes):
+        hash = hash.value
+
+    if args is None:
+        args = []
+
+    if download:
+        args.append("--download")
+
+    if checkfile is not None:
+        args.append(f'--checkfile "{checkfile}"')
+
+    if output_file is not None:
+        args.append(f'--output-file "{output_file}"')
+
+    process: str = utils.run_cmd(f'rclone hashsum "{hash}" "{path}"', args)
+
+    lines = process.stdout.splitlines()
+
+    exception = False
+
+    if process.returncode != 0:
+        if checkfile is None:
+            exception = True
+        else:
+            # validate that the checkfile command succeeded, by checking if the output has the expected form
+            for l in lines:
+                if not (l.startswith("= ") or l.startswith("* ")):
+                    exception = True
+                    break
+
+    if exception:
+        raise Exception(
+            f"hashsum operation on {path} with hash='{hash}' failed with:\n{process.stderr}"
+        )
+
+    if output_file is None:
+        # each line contains the hashsum first, followed by the name of the file
+        hashsums = {}
+
+        for l in lines:
+            if len(l) > 0:
+                value, key = l.split()
+
+                if checkfile is None:
+                    hashsums[key] = value
+                else:
+                    # in checkfile mode, value is '=' for valid and '*' for invalid files
+                    hashsums[key] = value == "="
+
+        # for only a single file return the value instead of the dict
+        if len(hashsums) == 1:
+            return next(iter(hashsums.values()))
+
+        return hashsums
+
+
+@__check_installed
+def version(
+    check=False,
+    args: List[str] = None,
+) -> Union[str, List[str]]:
+    """Get the rclone version number.
+
+    Args:
+        check (bool, optional): Whether to do an online check to compare your version with the latest release and the latest beta. Defaults to False.
+        args (List[str], optional): Optional additional list of flags. Defaults to None.
+
+    Returns:
+        Union[str, Set[str, str, str]]: When check is False, returns string of current version. When check is True returns installed version, lastest version and latest beta version.
+    """
+    if args is None:
+        args = []
+
+    if check:
+        args.append("--check")
+
+    process = utils.run_cmd("rclone version", args)
+
+    if process.returncode != 0:
+        raise Exception(process.stderr)
+
+    stdout = process.stdout
+
+    if not check:
+        return stdout.split("\n")[0].replace("rclone ", "")
+    else:
+        yours = re.findall(r"yours:\s+([\d.]+)", stdout)[0]
+        latest = re.findall(r"latest:\s+([\d.]+)", stdout)[0]
+        # beta version might include dashes and word characters e.g. '1.64.0-beta.7161.9169b2b5a'
+        beta = re.findall(r"beta:\s+([.\w-]+)", stdout)[0]
+        return yours, latest, beta
+
+
+@__check_installed
 def _rclone_transfer_operation(
     in_path: str,
     out_path: str,
     command: str,
     command_descr: str,
     ignore_existing=False,
     show_progress=True,
```

### Comparing `rclone-python-0.1.8/rclone_python/remote_types.py` & `rclone-python-0.1.9/rclone_python/remote_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 
 
 class RemoteTypes(Enum):
-    """These are all the cloud systems support by rclone (generated with v1.62.2).
+    """These are all the cloud systems support by rclone (generated with v1.63.1).
     A more detailed overview can be found here: https://rclone.org/overview/
     """
 
     amazon_cloud_drive = "amazon cloud drive"
     azureblob = "azureblob"
     b2 = "b2"
     box = "box"
@@ -34,14 +34,15 @@
     mega = "mega"
     memory = "memory"
     netstorage = "netstorage"
     onedrive = "onedrive"
     opendrive = "opendrive"
     oracleobjectstorage = "oracleobjectstorage"
     pcloud = "pcloud"
+    pikpak = "pikpak"
     premiumizeme = "premiumizeme"
     putio = "putio"
     qingstor = "qingstor"
     s3 = "s3"
     seafile = "seafile"
     sftp = "sftp"
     sharefile = "sharefile"
```

### Comparing `rclone-python-0.1.8/rclone_python/utils.py` & `rclone-python-0.1.9/rclone_python/utils.py`

 * *Files identical despite different names*

### Comparing `rclone-python-0.1.8/rclone_python.egg-info/PKG-INFO` & `rclone-python-0.1.9/rclone_python.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclone-python
-Version: 0.1.8
+Version: 0.1.9
 Summary: A python wrapper for rclone.
 Home-page: https://github.com/Johannes11833/rclone_python
 Author: Johannes Gundlach
 Keywords: rclone,wrapper,cloud sync
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,16 +24,19 @@
 
 ## Features ⚒️
 
 - Copy, move and sync files between remotes
 - Delete and prune files/directories
 - List files in a directory including properties of the files.
 - List available remotes.
+- Generate hashes from files or validate them with their hashsum.
 - Create new remotes
 - Check available remotes
+- Create and manage public links.
+- Check the currently installed rclone versions and if updates are available.
 
 ## Installation 💾
 
 _rclone_python_ can be installed using pip
 
 ```shell
 pip install rclone-python
@@ -106,7 +109,15 @@
 ```python
 from rclone_python import rclone
 
 # remove the entire test_dir folder (and all files contained in it and it's subdirectories) on onedrive
 rclone.purge('onedrive:test_dir')
 ```
 
+### Get Hash
+```python
+from rclone_python import rclone
+from rclone_python.hash_types import HashTypes
+
+print(rclone.hash(HashTypes.sha1, "box:data")
+# {'video1.webm': '3ef08d895f25e8b7d84d3a1ac58f8f302e33058b', 'video3.webm': '3ef08d895f25e8b7d84d3a1ac58f8f302e33058b', 'video2.webm': '3ef08d895f25e8b7d84d3a1ac58f8f302e33058b'}
+```
```

### Comparing `rclone-python-0.1.8/setup.py` & `rclone-python-0.1.9/setup.py`

 * *Files identical despite different names*

