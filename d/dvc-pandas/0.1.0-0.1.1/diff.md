# Comparing `tmp/dvc-pandas-0.1.0.tar.gz` & `tmp/dvc-pandas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-pandas-0.1.0.tar", last modified: Tue Apr 11 16:37:11 2023, max compression
+gzip compressed data, was "dvc-pandas-0.1.1.tar", last modified: Wed Jul 26 16:43:25 2023, max compression
```

## Comparing `dvc-pandas-0.1.0.tar` & `dvc-pandas-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/
--rw-rw-r--   0 jey       (1000) jey       (1000)     1068 2021-04-06 11:20:04.000000 dvc-pandas-0.1.0/LICENSE
--rw-rw-r--   0 jey       (1000) jey       (1000)      556 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/PKG-INFO
--rw-rw-r--   0 jey       (1000) jey       (1000)       13 2021-04-06 11:20:04.000000 dvc-pandas-0.1.0/README.md
--rw-rw-r--   0 jey       (1000) jey       (1000)      304 2022-02-09 06:54:41.000000 dvc-pandas-0.1.0/pyproject.toml
--rw-rw-r--   0 jey       (1000) jey       (1000)     1026 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/setup.cfg
--rw-rw-r--   0 jey       (1000) jey       (1000)      120 2021-04-06 11:20:04.000000 dvc-pandas-0.1.0/setup.py
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/src/
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/src/dvc_pandas/
--rw-rw-r--   0 jey       (1000) jey       (1000)      154 2021-06-12 14:42:57.000000 dvc-pandas-0.1.0/src/dvc_pandas/__init__.py
--rw-rw-r--   0 jey       (1000) jey       (1000)     3606 2023-01-24 20:05:52.000000 dvc-pandas-0.1.0/src/dvc_pandas/dataset.py
--rw-rw-r--   0 jey       (1000) jey       (1000)      352 2021-06-12 14:42:57.000000 dvc-pandas-0.1.0/src/dvc_pandas/dvc.py
--rw-rw-r--   0 jey       (1000) jey       (1000)     2705 2023-04-11 14:35:40.000000 dvc-pandas-0.1.0/src/dvc_pandas/git.py
--rw-rw-r--   0 jey       (1000) jey       (1000)    13448 2023-04-11 16:35:22.000000 dvc-pandas-0.1.0/src/dvc_pandas/repository.py
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/
--rw-rw-r--   0 jey       (1000) jey       (1000)      556 2023-04-11 16:37:11.000000 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 jey       (1000) jey       (1000)      413 2023-04-11 16:37:11.000000 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 jey       (1000) jey       (1000)        1 2023-04-11 16:37:11.000000 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 jey       (1000) jey       (1000)       92 2023-04-11 16:37:11.000000 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/requires.txt
--rw-rw-r--   0 jey       (1000) jey       (1000)       11 2023-04-11 16:37:11.000000 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/top_level.txt
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/tests/
--rw-rw-r--   0 jey       (1000) jey       (1000)      941 2021-10-08 15:22:36.000000 dvc-pandas-0.1.0/tests/test_dataset.py
--rw-rw-r--   0 jey       (1000) jey       (1000)     7606 2021-06-12 14:42:57.000000 dvc-pandas-0.1.0/tests/test_repository.py
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/
+-rw-rw-r--   0 jey       (1000) jey       (1000)     1068 2021-04-06 11:20:04.000000 dvc-pandas-0.1.1/LICENSE
+-rw-rw-r--   0 jey       (1000) jey       (1000)      556 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/PKG-INFO
+-rw-rw-r--   0 jey       (1000) jey       (1000)       13 2021-04-06 11:20:04.000000 dvc-pandas-0.1.1/README.md
+-rw-rw-r--   0 jey       (1000) jey       (1000)      304 2022-02-09 06:54:41.000000 dvc-pandas-0.1.1/pyproject.toml
+-rw-rw-r--   0 jey       (1000) jey       (1000)     1025 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/setup.cfg
+-rw-rw-r--   0 jey       (1000) jey       (1000)      120 2021-04-06 11:20:04.000000 dvc-pandas-0.1.1/setup.py
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/src/
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/src/dvc_pandas/
+-rw-rw-r--   0 jey       (1000) jey       (1000)      154 2021-06-12 14:42:57.000000 dvc-pandas-0.1.1/src/dvc_pandas/__init__.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)     3606 2023-07-26 16:41:53.000000 dvc-pandas-0.1.1/src/dvc_pandas/dataset.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)      352 2021-06-12 14:42:57.000000 dvc-pandas-0.1.1/src/dvc_pandas/dvc.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)     2705 2023-04-11 14:35:40.000000 dvc-pandas-0.1.1/src/dvc_pandas/git.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)    13396 2023-07-26 16:38:54.000000 dvc-pandas-0.1.1/src/dvc_pandas/repository.py
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-26 16:43:25.699135 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/
+-rw-rw-r--   0 jey       (1000) jey       (1000)      556 2023-07-26 16:43:25.000000 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 jey       (1000) jey       (1000)      366 2023-07-26 16:43:25.000000 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)        1 2023-07-26 16:43:25.000000 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)       91 2023-07-26 16:43:25.000000 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/requires.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)       11 2023-07-26 16:43:25.000000 dvc-pandas-0.1.1/src/dvc_pandas.egg-info/top_level.txt
```

### Comparing `dvc-pandas-0.1.0/LICENSE` & `dvc-pandas-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-pandas-0.1.0/PKG-INFO` & `dvc-pandas-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-pandas
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper for DVC and git to easily fetch Pandas dataframes
 Home-page: https://github.com/kausaltech/dvc-pandas
 Author: Bernhard Bliem
 Author-email: bernhard.bliem@kausal.tech
 Project-URL: Bug Tracker, https://github.com/kausaltech/dvc-pandas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dvc-pandas-0.1.0/setup.cfg` & `dvc-pandas-0.1.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dvc-pandas
-version = 0.1.0
+version = 0.1.1
 author = Bernhard Bliem
 author_email = bernhard.bliem@kausal.tech
 description = Wrapper for DVC and git to easily fetch Pandas dataframes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kausaltech/dvc-pandas
 project_urls = 
@@ -20,15 +20,15 @@
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	GitPython
 	appdirs
 	dvc
 	dvc-s3
-	fasteners
+	filelock
 	pyarrow
 	pandas
 	pint-pandas
 	python-snappy
 	ruamel.yaml
 
 [options.packages.find]
```

### Comparing `dvc-pandas-0.1.0/src/dvc_pandas/dataset.py` & `dvc-pandas-0.1.1/src/dvc_pandas/dataset.py`

 * *Files identical despite different names*

### Comparing `dvc-pandas-0.1.0/src/dvc_pandas/git.py` & `dvc-pandas-0.1.1/src/dvc_pandas/git.py`

 * *Files identical despite different names*

### Comparing `dvc-pandas-0.1.0/src/dvc_pandas/repository.py` & `dvc-pandas-0.1.1/src/dvc_pandas/repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 import git
 import gitdb
 import logging
 import os
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
-import fasteners
+import filelock
 import pandas as pd
 from ruamel.yaml import YAML
 
 import dvc.repo
 
 from .dataset import Dataset
 from .dvc import set_dvc_file_metadata
@@ -27,72 +27,65 @@
 class TemporaryGitCheckout:
     def __init__(self, repo: GitRepo, commit_id: str | None = None):
         self.repo = repo
         self.commit_id = commit_id
         self.original_branch = None
 
     def __enter__(self):
-        if self.commit_id:
-            try:
-                self.original_branch = self.repo.active_branch
-            except TypeError:
-                self.original_branch = None
-
-            try:
-                self.repo.head.reference = self.repo.commit(self.commit_id)
-            except (git.exc.BadName, gitdb.exc.BadObject, ValueError, IndexError):
-                logger.debug("Commit does not exist; pull and retry")
-                # Commit doesn't exist, try to pull and see what happens
-                self.repo.remote().pull()
-                self.repo.head.reference = self.repo.commit(self.commit_id)
-            self.repo.head.reset(index=True, working_tree=True)
-            # TODO: Pull if commit ID doesn't exist? Flag for enabling this beha
+        if not self.commit_id:
+            return
+
+        if self.repo.head.commit.hexsha == self.commit_id:
+            return
+
+        try:
+            self.original_branch = self.repo.active_branch
+        except TypeError:
+            self.original_branch = None
+
+        try:
+            self.repo.head.reference = self.repo.commit(self.commit_id)
+        except (git.exc.BadName, gitdb.exc.BadObject, ValueError, IndexError):
+            logger.debug("Commit does not exist; pull and retry")
+            # Commit doesn't exist, try to pull and see what happens
+            self.repo.remote().pull()
+            self.repo.head.reference = self.repo.commit(self.commit_id)
+        self.repo.head.reset(index=True, working_tree=True)
 
     def __exit__(self, *exc):
         if self.original_branch:
             self.original_branch.checkout()
 
 
 class ReentrantLock:
     """Lock that keeps track of invocations."""
-    process_lock: fasteners.InterProcessLock
-    thread_lock: fasteners.ReaderWriterLock
+    _lock: filelock.FileLock
 
     def __init__(self, lock_file: str):
-        self.process_lock = fasteners.InterProcessLock(lock_file)
-        self.thread_lock = fasteners.ReaderWriterLock()
-        self.acquisition_count = 0
-
-    @contextmanager
-    def lock(self):
-        with self.thread_lock.write_lock():
-            if not self.acquisition_count:
-                self.process_lock.acquire()
-            self.acquisition_count += 1
-            yield
-            assert self.acquisition_count >= 1
-            self.acquisition_count -= 1
-            if not self.acquisition_count:
-                self.process_lock.release()
+        self.lock = filelock.FileLock(lock_file, thread_local=True)
+
 
 def ensure_repo_lock(func):
     """Wrap a Repository class method with a lock."""
     def acquire_lock(self: Repository, *args, **kwargs):
-        with self.lock.lock():
+        with self.lock.lock.acquire():
             return func(self, *args, **kwargs)
 
     return acquire_lock
 
 
 class DatasetStageItem:
     def __init__(self, dataset):
         self.identifier = dataset.identifier
         self.metadata = dataset.dvc_metadata
 
 
+dataset_hash_cache: dict[str, Tuple[int, str]] = {}
+
+
 class Repository:
     dvc_remote: Optional[str]
     repo_url: str
     target_commit_id: Optional[str]
     dataset_stage: List[DatasetStageItem]
     git_repo: GitRepo
     dvc_repo: dvc.repo.Repo
@@ -121,36 +114,52 @@
         self.dataset_stage = []
         self.target_commit_id = None
         self.lock = ReentrantLock(str(self.repo_dir / '.dvc-pandas.lock'))
 
     def log_info(self, message: str):
         logger.info('[%s] %s' % (self.repo_url, message))
 
+    def acquire_lock(self):
+        self.lock.lock.acquire()
+
+    def release_lock(self):
+        self.lock.lock.release()
+
     @ensure_repo_lock
     def load_dataset(self, identifier: str, skip_pull_if_exists=False) -> Dataset:
         """
         Load dataset with the given identifier from the given repository.
 
         If `skip_pull_if_exists` is True, does not update the dataset if a parquet file exists for the identifier,
         regardless of the content.
         """
         def should_pull(parquet_path: Path, metadata: dict):
             if not skip_pull_if_exists:
                 return True
             if not parquet_path.exists():
                 return True
+            st = parquet_path.stat()
+            mtime = st.st_mtime_ns
             m = metadata['outs'][0]
-            if parquet_path.stat().st_size != m['size']:
+            if st.st_size != m['size']:
                 self.log_info(f"Size mismatch with {parquet_path}")
                 return True
-            with open(parquet_path, 'rb') as f:
-                h = md5(f.read()).hexdigest()
-                if h != m['md5']:
-                    self.log_info(f"MD5 hash mismatch with {parquet_path}")
-                    return True
+
+            cached = dataset_hash_cache.get(str(parquet_path))
+            if cached is not None and cached[0] == mtime:
+                dataset_hash = cached[1]
+            else:
+                with open(parquet_path, 'rb') as f:
+                    dataset_hash = md5(f.read()).hexdigest()
+                dataset_hash_cache[str(parquet_path)] = (mtime, dataset_hash)
+
+            if dataset_hash != m['md5']:
+                self.log_info(f"MD5 hash mismatch with {parquet_path}")
+                return True
+
             return False
 
         with TemporaryGitCheckout(self.git_repo, self.target_commit_id):
             parquet_path = self.repo_dir / (identifier + '.parquet')
 
             # Get metadata (including units) from .dvc file
             dvc_file_path = parquet_path.parent / (parquet_path.name + '.dvc')
```

### Comparing `dvc-pandas-0.1.0/src/dvc_pandas.egg-info/PKG-INFO` & `dvc-pandas-0.1.1/src/dvc_pandas.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-pandas
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper for DVC and git to easily fetch Pandas dataframes
 Home-page: https://github.com/kausaltech/dvc-pandas
 Author: Bernhard Bliem
 Author-email: bernhard.bliem@kausal.tech
 Project-URL: Bug Tracker, https://github.com/kausaltech/dvc-pandas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

