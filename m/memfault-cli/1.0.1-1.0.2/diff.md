# Comparing `tmp/memfault_cli-1.0.1.tar.gz` & `tmp/memfault_cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memfault_cli-1.0.1.tar", max compression
+gzip compressed data, was "memfault_cli-1.0.2.tar", max compression
```

## Comparing `memfault_cli-1.0.1.tar` & `memfault_cli-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3001 2023-07-06 15:16:06.787752 memfault_cli-1.0.1/README.md
--rw-r--r--   0        0        0       79 2023-05-30 21:30:22.282085 memfault_cli-1.0.1/memfault_cli/__init__.py
--rw-r--r--   0        0        0      529 2023-05-30 21:30:22.282144 memfault_cli-1.0.1/memfault_cli/_version.py
--rw-r--r--   0        0        0     2579 2023-05-30 21:30:22.282205 memfault_cli-1.0.1/memfault_cli/authenticator.py
--rw-r--r--   0        0        0     3895 2023-07-05 14:30:20.686261 memfault_cli-1.0.1/memfault_cli/chunk.py
--rw-r--r--   0        0        0    27792 2023-06-14 14:38:09.606809 memfault_cli-1.0.1/memfault_cli/cli.py
--rw-r--r--   0        0        0     9759 2023-05-30 21:30:22.282483 memfault_cli-1.0.1/memfault_cli/console.py
--rw-r--r--   0        0        0    13111 2023-06-22 19:07:02.890559 memfault_cli-1.0.1/memfault_cli/context.py
--rw-r--r--   0        0        0     4765 2023-07-05 14:30:20.686386 memfault_cli-1.0.1/memfault_cli/deploy.py
--rw-r--r--   0        0        0     4115 2023-05-30 21:30:22.282688 memfault_cli-1.0.1/memfault_cli/elf.py
--rw-r--r--   0        0        0      633 2023-05-30 21:30:22.282740 memfault_cli-1.0.1/memfault_cli/functools_ext.py
--rw-r--r--   0        0        0    26113 2023-07-06 15:16:06.788088 memfault_cli-1.0.1/memfault_cli/upload.py
--rw-r--r--   0        0        0     7775 2023-07-05 13:14:43.930272 memfault_cli-1.0.1/memfault_cli/yocto.py
--rw-r--r--   0        0        0     3528 2023-07-06 15:16:06.788346 memfault_cli-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4192 1970-01-01 00:00:00.000000 memfault_cli-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3146 2023-07-26 13:56:44.992237 memfault_cli-1.0.2/README.md
+-rw-r--r--   0        0        0       79 2022-11-29 21:27:02.913006 memfault_cli-1.0.2/memfault_cli/__init__.py
+-rw-r--r--   0        0        0      529 2023-02-13 17:39:09.827340 memfault_cli-1.0.2/memfault_cli/_version.py
+-rw-r--r--   0        0        0     2579 2023-03-27 16:07:26.510250 memfault_cli-1.0.2/memfault_cli/authenticator.py
+-rw-r--r--   0        0        0     3895 2023-07-18 10:04:36.924224 memfault_cli-1.0.2/memfault_cli/chunk.py
+-rw-r--r--   0        0        0    27792 2023-06-12 22:08:59.785313 memfault_cli-1.0.2/memfault_cli/cli.py
+-rw-r--r--   0        0        0     9759 2023-05-22 17:29:50.252914 memfault_cli-1.0.2/memfault_cli/console.py
+-rw-r--r--   0        0        0    13111 2023-06-12 22:08:59.785520 memfault_cli-1.0.2/memfault_cli/context.py
+-rw-r--r--   0        0        0     4765 2023-07-18 10:04:36.924384 memfault_cli-1.0.2/memfault_cli/deploy.py
+-rw-r--r--   0        0        0     4115 2022-11-29 21:27:02.913672 memfault_cli-1.0.2/memfault_cli/elf.py
+-rw-r--r--   0        0        0      633 2022-11-29 21:27:02.913734 memfault_cli-1.0.2/memfault_cli/functools_ext.py
+-rw-r--r--   0        0        0    26113 2023-07-18 10:04:36.924578 memfault_cli-1.0.2/memfault_cli/upload.py
+-rw-r--r--   0        0        0     7923 2023-07-26 13:28:27.916144 memfault_cli-1.0.2/memfault_cli/yocto.py
+-rw-r--r--   0        0        0     3528 2023-07-26 13:56:44.992666 memfault_cli-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4337 1970-01-01 00:00:00.000000 memfault_cli-1.0.2/PKG-INFO
```

### Comparing `memfault_cli-1.0.1/README.md` & `memfault_cli-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 The purpose of the tool is to make integration with Memfault from other systems,
 like continuous integration servers, as easy as possible.
 
 Install the tool and run `memfault --help` for more info!
 
 ## Changes
 
+### 1.0.2
+
+- Fix a bug where `upload-yocto-symbols` would fail when some files in the
+  tarballs provided did not have the read permission set.
+
 ### 1.0.1
 
 - Fix `upload-custom-data-recording` to print a more helpful error message when
   exceeding device rate limits.
 
 ### 1.0.0
```

### Comparing `memfault_cli-1.0.1/memfault_cli/_version.py` & `memfault_cli-1.0.2/memfault_cli/_version.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.1/memfault_cli/authenticator.py` & `memfault_cli-1.0.2/memfault_cli/authenticator.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.1/memfault_cli/chunk.py` & `memfault_cli-1.0.2/memfault_cli/chunk.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.1/memfault_cli/cli.py` & `memfault_cli-1.0.2/memfault_cli/cli.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.1/memfault_cli/console.py` & `memfault_cli-1.0.2/memfault_cli/console.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.1/memfault_cli/context.py` & `memfault_cli-1.0.2/memfault_cli/context.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.1/memfault_cli/deploy.py` & `memfault_cli-1.0.2/memfault_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.1/memfault_cli/elf.py` & `memfault_cli-1.0.2/memfault_cli/elf.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.1/memfault_cli/functools_ext.py` & `memfault_cli-1.0.2/memfault_cli/functools_ext.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.1/memfault_cli/upload.py` & `memfault_cli-1.0.2/memfault_cli/upload.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.1/memfault_cli/yocto.py` & `memfault_cli-1.0.2/memfault_cli/yocto.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 
 def find_elf_files_from_image(image_tar: pathlib.Path) -> Iterable[ELFFileInfo]:
     with tarfile.open(
         image_tar, "r:*"
     ) as tar, tempfile.TemporaryDirectory() as extraction_path_str:
         tar.extractall(extraction_path_str)
+        subprocess.check_call(["chmod", "u+r", "-R", extraction_path_str])
         extraction_path = pathlib.Path(extraction_path_str)
         yield from find_elf_files(extraction_path, relative_to=extraction_path)
 
 
 # https://docs.yoctoproject.org/ref-manual/variables.html?highlight=package_debug_split_style#term-PACKAGE_DEBUG_SPLIT_STYLE
 class PackageDebugSplitStyle(Enum):
     DEBUG = ".debug"
@@ -180,14 +181,15 @@
         missing_infos: List[ELFFileInfo] = []
 
         debug_symbols_dir = workbench_dir / "debug"
         debug_symbols_dir.mkdir()
 
         click.echo(f"Extracting debug symbols ({dbg_image_size_mb} MB) to a temporary directory...")
         debug_image_tar.extractall(debug_symbols_dir)
+        subprocess.check_call(["chmod", "u+r", "-R", debug_symbols_dir])
 
         for elf_info in _image_elfs(image):
             if "/lib/modules" in str(elf_info.path):
                 # Not interested in kernel modules and we don't have debug
                 # symbols for those anyway.
                 continue
```

### Comparing `memfault_cli-1.0.1/pyproject.toml` & `memfault_cli-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "memfault-cli"
-version = "1.0.1"
+version = "1.0.2"
 description = "Memfault CLI tool"
 homepage = "https://docs.memfault.com"
 documentation = "https://docs.memfault.com/docs/ci/install-memfault-cli"
 authors = ["Memfault Inc <hello@memfault.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `memfault_cli-1.0.1/PKG-INFO` & `memfault_cli-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memfault-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: Memfault CLI tool
 Home-page: https://docs.memfault.com
 Author: Memfault Inc
 Author-email: hello@memfault.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -35,14 +35,19 @@
 The purpose of the tool is to make integration with Memfault from other systems,
 like continuous integration servers, as easy as possible.
 
 Install the tool and run `memfault --help` for more info!
 
 ## Changes
 
+### 1.0.2
+
+- Fix a bug where `upload-yocto-symbols` would fail when some files in the
+  tarballs provided did not have the read permission set.
+
 ### 1.0.1
 
 - Fix `upload-custom-data-recording` to print a more helpful error message when
   exceeding device rate limits.
 
 ### 1.0.0
```

