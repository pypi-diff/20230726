# Comparing `tmp/eztils-0.4.72.tar.gz` & `tmp/eztils-0.4.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztils-0.4.72.tar", max compression
+gzip compressed data, was "eztils-0.4.73.tar", max compression
```

## Comparing `eztils-0.4.72.tar` & `eztils-0.4.73.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1075 2023-07-24 06:58:03.175239 eztils-0.4.72/LICENSE
--rw-r--r--   0        0        0    12741 2023-07-24 06:58:03.179240 eztils-0.4.72/README.md
--rw-r--r--   0        0        0      542 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/__init__.py
--rw-r--r--   0        0        0     2494 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/__init__.py
--rw-r--r--   0        0        0     3689 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/dict_operations.py
--rw-r--r--   0        0        0     2246 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/itertools.py
--rw-r--r--   0        0        0     2458 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/logging.py
--rw-r--r--   0        0        0     1432 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/math.py
--rw-r--r--   0        0        0     2812 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/serialization.py
--rw-r--r--   0        0        0     1091 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/default/structures.py
--rw-r--r--   0        0        0     4296 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/git/__init__.py
--rw-r--r--   0        0        0     1779 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/__init__.py
--rw-r--r--   0        0        0    15646 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/distributions.py
--rw-r--r--   0        0        0      155 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/lightning.py
--rw-r--r--   0        0        0      173 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/math.py
--rw-r--r--   0        0        0     2550 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/modules.py
--rw-r--r--   0        0        0     1420 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/parameters.py
--rw-r--r--   0        0        0     1746 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/tensor_creators.py
--rw-r--r--   0        0        0     3001 2023-07-24 06:58:03.179240 eztils-0.4.72/eztils/torch/to.py
--rw-r--r--   0        0        0     3611 2023-07-24 06:58:03.179240 eztils-0.4.72/pyproject.toml
--rw-r--r--   0        0        0    13946 1970-01-01 00:00:00.000000 eztils-0.4.72/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-26 02:41:51.330459 eztils-0.4.73/LICENSE
+-rw-r--r--   0        0        0    12741 2023-07-26 02:41:51.330459 eztils-0.4.73/README.md
+-rw-r--r--   0        0        0      542 2023-07-26 02:41:51.330459 eztils-0.4.73/eztils/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-26 02:41:51.330459 eztils-0.4.73/eztils/default/__init__.py
+-rw-r--r--   0        0        0     3689 2023-07-26 02:41:51.330459 eztils-0.4.73/eztils/default/dict_operations.py
+-rw-r--r--   0        0        0     2246 2023-07-26 02:41:51.330459 eztils-0.4.73/eztils/default/itertools.py
+-rw-r--r--   0        0        0     2458 2023-07-26 02:41:51.330459 eztils-0.4.73/eztils/default/logging.py
+-rw-r--r--   0        0        0     1432 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/default/math.py
+-rw-r--r--   0        0        0     2812 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/default/serialization.py
+-rw-r--r--   0        0        0     1091 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/default/structures.py
+-rw-r--r--   0        0        0     4619 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/git/__init__.py
+-rw-r--r--   0        0        0     1812 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/torch/__init__.py
+-rw-r--r--   0        0        0    15646 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/torch/distributions.py
+-rw-r--r--   0        0        0      155 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/torch/lightning.py
+-rw-r--r--   0        0        0      173 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/torch/math.py
+-rw-r--r--   0        0        0     2550 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/torch/modules.py
+-rw-r--r--   0        0        0     1420 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/torch/parameters.py
+-rw-r--r--   0        0        0     1935 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/torch/tensor_creators.py
+-rw-r--r--   0        0        0     3001 2023-07-26 02:41:51.334459 eztils-0.4.73/eztils/torch/to.py
+-rw-r--r--   0        0        0     3611 2023-07-26 02:41:51.334459 eztils-0.4.73/pyproject.toml
+-rw-r--r--   0        0        0    13946 1970-01-01 00:00:00.000000 eztils-0.4.73/PKG-INFO
```

### Comparing `eztils-0.4.72/LICENSE` & `eztils-0.4.73/LICENSE`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/README.md` & `eztils-0.4.73/README.md`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/__init__.py` & `eztils-0.4.73/eztils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/default/__init__.py` & `eztils-0.4.73/eztils/default/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/default/dict_operations.py` & `eztils-0.4.73/eztils/default/dict_operations.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/default/itertools.py` & `eztils-0.4.73/eztils/default/itertools.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/default/logging.py` & `eztils-0.4.73/eztils/default/logging.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/default/math.py` & `eztils-0.4.73/eztils/default/math.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/default/serialization.py` & `eztils-0.4.73/eztils/default/serialization.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/default/structures.py` & `eztils-0.4.73/eztils/default/structures.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/git/__init__.py` & `eztils-0.4.73/eztils/git/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,23 +19,23 @@
         "branch_name",
     ],
 )
 
 
 def copyanything(src, dst):
     try:
-        shutil.copytree(src, dst)
+        shutil.copytree(src, dst, ignore=shutil.ignore_patterns("lfs"))
     except OSError as exc:  # python >2.5
         if exc.errno in (errno.ENOTDIR, errno.EINVAL):
             shutil.copy(src, dst)
         else:
             raise
 
 
-def copy_git_repo(root: str, dest_path: str):
+def copy_git_repo(root: str, dest_path: str, exclude: list = None):
     """Given a destination path, copy the local root dir to the path.
     This function can be used to generate a snapshot of the repo so that the
     exactly same code status will be recovered when later playing a trained
     model or launching a grid-search job in the waiting queue.
     Args:
         root (str): the path to the repo
         dest_path (str): the path to generate a snapshot of repo
@@ -48,16 +48,22 @@
         cwd=root_path,
         capture_output=True,
         text=True,
     ).stdout.splitlines()
 
     # Create the destination directory if it doesn't exist
     dest_path.mkdir(parents=True, exist_ok=True)
-
     # Copy files to destination, preserving directory structure
+
+    # remove excluded
+    if exclude is not None:
+        for e in exclude:
+            if e in files:
+                files.remove(e)
+
     for src_file in files:
         src_file = Path(src_file)
         dest_file = dest_path / src_file
         # Create necessary directories in destination
         dest_file.parent.mkdir(parents=True, exist_ok=True)
 
         src = root_path / src_file
@@ -68,25 +74,26 @@
         copyanything(root_path / src_file, dest_file)
 
     copyanything(root_path / ".git", dest_path / ".git")
 
     # Recursively process submodules
     root_repo = Repo(root)
     submodules = get_submodules(root_repo)
-
     for submodule in submodules:
         # Call copy_git_repo recursively on the submodule
+        if any([e in submodule.working_tree_dir for e in exclude]):
+            continue
         copy_git_repo(
             submodule.working_tree_dir,
             dest_path / Path(submodule.working_tree_dir).relative_to(root_path),
         )
 
 
-def generate_snapshot(root: str, dest_path: str):
-    copy_git_repo(root, dest_path)
+def generate_snapshot(root: str, dest_path: str, exclude: list = None):
+    copy_git_repo(root, dest_path, exclude=exclude)
     dest_path = Path(dest_path)
 
     root_repo = Repo(root)
     submodules = get_submodules_recursively(root_repo)
 
     git_infos = [get_git_info(i.working_tree_dir) for i in [root_repo] + submodules]
     for directory, code_diff, code_diff_staged, commit_hash, branch_name in git_infos:
```

### Comparing `eztils-0.4.72/eztils/torch/__init__.py` & `eztils-0.4.73/eztils/torch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,19 @@
         torch.cuda.manual_seed_all(seed)
 
 
 save = partial(save, save_fn=torch.save)
 torch.load = partial(torch.load, map_location="cpu")
 load = partial(load, load_fn=torch.load)
 
+
+def identity(x):
+    return x
+
+
 from .distributions import *
 from .lightning import *
 from .math import *
 from .modules import *
 from .parameters import *
 from .tensor_creators import *
 from .to import *
```

### Comparing `eztils-0.4.72/eztils/torch/distributions.py` & `eztils-0.4.73/eztils/torch/distributions.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/torch/modules.py` & `eztils-0.4.73/eztils/torch/modules.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/torch/parameters.py` & `eztils-0.4.73/eztils/torch/parameters.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/eztils/torch/tensor_creators.py` & `eztils-0.4.73/eztils/torch/tensor_creators.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,29 +3,34 @@
 """
 import torch
 
 from eztils import default
 
 
 def device_dtype_decorator(func):
-    def wrapper(*args, torch_device=None, **kwargs):
+    def wrapper(*args, **kwargs):
         from eztils.torch import DEVICE, DTYPE
 
-        torch_device = default(torch_device, DEVICE)
+        torch_device = default(kwargs.get("device"), DEVICE)
         torch_dtype = default(kwargs.get("dtype"), DTYPE)
         kwargs.pop("device", None)
         kwargs.pop("dtype", None)
         return func(*args, **kwargs, device=torch_device, dtype=torch_dtype)
 
     return wrapper
 
 
-@device_dtype_decorator
-def from_numpy(*args, **kwargs):
-    return torch.from_numpy(*args, **kwargs)
+# torch.from_numpy doesn't support kwargs
+def from_numpy(np_array, device=None, dtype=None):
+    from eztils.torch import DEVICE, DTYPE
+
+    torch_device = default(device, DEVICE)
+    torch_dtype = default(dtype, DTYPE)
+
+    return torch.from_numpy(np_array).to(device=torch_device, dtype=torch_dtype)
 
 
 @device_dtype_decorator
 def tensor(*args, **kwargs):
     return torch.tensor(*args, **kwargs)
```

### Comparing `eztils-0.4.72/eztils/torch/to.py` & `eztils-0.4.73/eztils/torch/to.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.72/pyproject.toml` & `eztils-0.4.73/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
 description = "eds utilities"
 homepage = "https://github.com/ezhang7423/eztils"
 license = "MIT"
 name = "eztils"
 readme = "README.md"
 repository = "https://github.com/ezhang7423/eztils"
-version = "0.4.72"
+version = "0.4.73"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `eztils-0.4.72/PKG-INFO` & `eztils-0.4.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eztils
-Version: 0.4.72
+Version: 0.4.73
 Summary: eds utilities
 Home-page: https://github.com/ezhang7423/eztils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

