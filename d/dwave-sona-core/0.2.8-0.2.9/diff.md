# Comparing `tmp/dwave_sona_core-0.2.8.tar.gz` & `tmp/dwave_sona_core-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave_sona_core-0.2.8.tar", max compression
+gzip compressed data, was "dwave_sona_core-0.2.9.tar", max compression
```

## Comparing `dwave_sona_core-0.2.8.tar` & `dwave_sona_core-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1085 2023-06-06 06:28:04.762478 dwave_sona_core-0.2.8/LICENSE
--rw-r--r--   0        0        0     3711 2023-06-06 06:26:51.725598 dwave_sona_core-0.2.8/README.md
--rw-r--r--   0        0        0      501 2023-06-06 06:25:53.680907 dwave_sona_core-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1875 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.8/sona/__init__.py
--rw-r--r--   0        0        0       59 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/__main__.py
--rw-r--r--   0        0        0      544 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.8/sona/core/consumers/__init__.py
--rw-r--r--   0        0        0      223 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/consumers/base.py
--rw-r--r--   0        0        0      794 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/consumers/kafka.py
--rw-r--r--   0        0        0     1173 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/consumers/redis.py
--rw-r--r--   0        0        0      924 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/consumers/sqs.py
--rw-r--r--   0        0        0      227 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/messages/__init__.py
--rw-r--r--   0        0        0      340 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/messages/base.py
--rw-r--r--   0        0        0     1512 2023-05-29 09:56:04.536351 dwave_sona_core-0.2.8/sona/core/messages/context.py
--rw-r--r--   0        0        0      135 2023-06-02 03:25:59.908116 dwave_sona_core-0.2.8/sona/core/messages/file.py
--rw-r--r--   0        0        0     1756 2023-05-29 03:34:15.202108 dwave_sona_core-0.2.8/sona/core/messages/job.py
--rw-r--r--   0        0        0      353 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/messages/result.py
--rw-r--r--   0        0        0      785 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/messages/state.py
--rw-r--r--   0        0        0      614 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.8/sona/core/producers/__init__.py
--rw-r--r--   0        0        0      131 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/producers/base.py
--rw-r--r--   0        0        0      606 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/producers/kafka.py
--rw-r--r--   0        0        0      187 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/producers/mock.py
--rw-r--r--   0        0        0      331 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/producers/redis.py
--rw-r--r--   0        0        0      290 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/producers/sqs.py
--rw-r--r--   0        0        0      308 2023-05-29 03:37:39.760706 dwave_sona_core-0.2.8/sona/core/storages/__init__.py
--rw-r--r--   0        0        0     1458 2023-05-29 02:44:30.887610 dwave_sona_core-0.2.8/sona/core/storages/base.py
--rw-r--r--   0        0        0     1153 2023-05-29 02:44:30.907611 dwave_sona_core-0.2.8/sona/core/storages/local.py
--rw-r--r--   0        0        0     1687 2023-05-29 03:38:24.421273 dwave_sona_core-0.2.8/sona/core/storages/s3.py
--rw-r--r--   0        0        0        0 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/utils/__init__.py
--rw-r--r--   0        0        0      368 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/utils/cls_utils.py
--rw-r--r--   0        0        0      204 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/core/utils/dict_utils.py
--rw-r--r--   0        0        0       63 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/inferencers/__init__.py
--rw-r--r--   0        0        0      913 2023-05-29 02:44:30.907611 dwave_sona_core-0.2.8/sona/inferencers/base.py
--rw-r--r--   0        0        0     2095 2023-05-29 02:44:30.907611 dwave_sona_core-0.2.8/sona/inferencers/mock.py
--rw-r--r--   0        0        0     1738 2023-06-06 06:24:54.588212 dwave_sona_core-0.2.8/sona/settings.py
--rw-r--r--   0        0        0      116 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.8/sona/workers/__init__.py
--rw-r--r--   0        0        0     1957 2023-06-06 06:24:54.588212 dwave_sona_core-0.2.8/sona/workers/base.py
--rw-r--r--   0        0        0     2635 2023-05-29 02:44:30.919611 dwave_sona_core-0.2.8/sona/workers/inferencer.py
--rw-r--r--   0        0        0     4421 1970-01-01 00:00:00.000000 dwave_sona_core-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-06 06:42:06.909115 dwave_sona_core-0.2.9/LICENSE
+-rw-r--r--   0        0        0     3711 2023-07-26 10:01:09.561805 dwave_sona_core-0.2.9/README.md
+-rw-r--r--   0        0        0      501 2023-07-26 10:08:15.289302 dwave_sona_core-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1875 2023-07-26 10:01:09.573805 dwave_sona_core-0.2.9/sona/__init__.py
+-rw-r--r--   0        0        0       59 2023-07-05 08:20:57.685330 dwave_sona_core-0.2.9/sona/__main__.py
+-rw-r--r--   0        0        0      544 2023-07-26 10:01:09.573805 dwave_sona_core-0.2.9/sona/core/consumers/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.9/sona/core/consumers/base.py
+-rw-r--r--   0        0        0      794 2023-07-26 10:01:09.573805 dwave_sona_core-0.2.9/sona/core/consumers/kafka.py
+-rw-r--r--   0        0        0     1173 2023-07-26 10:01:09.573805 dwave_sona_core-0.2.9/sona/core/consumers/redis.py
+-rw-r--r--   0        0        0      924 2023-07-26 10:01:09.573805 dwave_sona_core-0.2.9/sona/core/consumers/sqs.py
+-rw-r--r--   0        0        0      227 2023-07-26 10:01:09.589805 dwave_sona_core-0.2.9/sona/core/messages/__init__.py
+-rw-r--r--   0        0        0      340 2023-07-26 10:01:09.589805 dwave_sona_core-0.2.9/sona/core/messages/base.py
+-rw-r--r--   0        0        0     1512 2023-07-26 10:01:09.589805 dwave_sona_core-0.2.9/sona/core/messages/context.py
+-rw-r--r--   0        0        0      135 2023-07-26 10:01:09.589805 dwave_sona_core-0.2.9/sona/core/messages/file.py
+-rw-r--r--   0        0        0     1756 2023-07-26 10:01:09.589805 dwave_sona_core-0.2.9/sona/core/messages/job.py
+-rw-r--r--   0        0        0      353 2023-07-26 10:01:09.589805 dwave_sona_core-0.2.9/sona/core/messages/result.py
+-rw-r--r--   0        0        0      785 2023-07-26 10:01:09.589805 dwave_sona_core-0.2.9/sona/core/messages/state.py
+-rw-r--r--   0        0        0      614 2023-07-26 10:01:09.589805 dwave_sona_core-0.2.9/sona/core/producers/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.9/sona/core/producers/base.py
+-rw-r--r--   0        0        0      606 2023-07-26 10:01:09.589805 dwave_sona_core-0.2.9/sona/core/producers/kafka.py
+-rw-r--r--   0        0        0      187 2023-07-26 10:01:09.589805 dwave_sona_core-0.2.9/sona/core/producers/mock.py
+-rw-r--r--   0        0        0      331 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.9/sona/core/producers/redis.py
+-rw-r--r--   0        0        0      290 2023-07-26 10:01:09.593805 dwave_sona_core-0.2.9/sona/core/producers/sqs.py
+-rw-r--r--   0        0        0      308 2023-07-26 10:01:09.605805 dwave_sona_core-0.2.9/sona/core/storages/__init__.py
+-rw-r--r--   0        0        0     1458 2023-07-26 10:01:09.609806 dwave_sona_core-0.2.9/sona/core/storages/base.py
+-rw-r--r--   0        0        0     1387 2023-07-26 10:06:04.252743 dwave_sona_core-0.2.9/sona/core/storages/local.py
+-rw-r--r--   0        0        0     1687 2023-07-26 10:01:09.613806 dwave_sona_core-0.2.9/sona/core/storages/s3.py
+-rw-r--r--   0        0        0        0 2023-07-26 10:01:09.613806 dwave_sona_core-0.2.9/sona/core/utils/__init__.py
+-rw-r--r--   0        0        0      368 2023-07-26 10:01:09.613806 dwave_sona_core-0.2.9/sona/core/utils/cls_utils.py
+-rw-r--r--   0        0        0      204 2023-07-26 10:01:09.613806 dwave_sona_core-0.2.9/sona/core/utils/dict_utils.py
+-rw-r--r--   0        0        0       63 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.9/sona/inferencers/__init__.py
+-rw-r--r--   0        0        0      913 2023-07-26 10:01:09.613806 dwave_sona_core-0.2.9/sona/inferencers/base.py
+-rw-r--r--   0        0        0     2095 2023-07-26 10:01:09.613806 dwave_sona_core-0.2.9/sona/inferencers/mock.py
+-rw-r--r--   0        0        0     1738 2023-07-26 10:01:09.621806 dwave_sona_core-0.2.9/sona/settings.py
+-rw-r--r--   0        0        0      116 2023-05-25 13:39:18.174828 dwave_sona_core-0.2.9/sona/workers/__init__.py
+-rw-r--r--   0        0        0     1957 2023-07-26 10:01:09.621806 dwave_sona_core-0.2.9/sona/workers/base.py
+-rw-r--r--   0        0        0     2635 2023-07-26 10:01:09.621806 dwave_sona_core-0.2.9/sona/workers/inferencer.py
+-rw-r--r--   0        0        0     4421 1970-01-01 00:00:00.000000 dwave_sona_core-0.2.9/PKG-INFO
```

### Comparing `dwave_sona_core-0.2.8/LICENSE` & `dwave_sona_core-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/README.md` & `dwave_sona_core-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/__init__.py` & `dwave_sona_core-0.2.9/sona/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/consumers/__init__.py` & `dwave_sona_core-0.2.9/sona/core/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/consumers/kafka.py` & `dwave_sona_core-0.2.9/sona/core/consumers/kafka.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/consumers/redis.py` & `dwave_sona_core-0.2.9/sona/core/consumers/redis.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/consumers/sqs.py` & `dwave_sona_core-0.2.9/sona/core/consumers/sqs.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/messages/context.py` & `dwave_sona_core-0.2.9/sona/core/messages/context.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/messages/job.py` & `dwave_sona_core-0.2.9/sona/core/messages/job.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/messages/state.py` & `dwave_sona_core-0.2.9/sona/core/messages/state.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/producers/__init__.py` & `dwave_sona_core-0.2.9/sona/core/producers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/producers/kafka.py` & `dwave_sona_core-0.2.9/sona/core/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/storages/base.py` & `dwave_sona_core-0.2.9/sona/core/storages/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/core/storages/local.py` & `dwave_sona_core-0.2.9/sona/core/storages/local.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import os
 import shutil
 from pathlib import Path
 
 from sona.core.storages.base import ShareStorageBase
 from sona.settings import settings
 
@@ -21,12 +22,17 @@
         tmp_path = os.path.relpath(path, self.local_root)
         Path(tmp_path).parent.mkdir(parents=True, exist_ok=True)
         with open(path, "rb") as f_in, open(tmp_path, "wb") as f_out:
             shutil.copyfileobj(f_in, f_out)
         return str(tmp_path)
 
     def on_push(self, path: str) -> str:
-        local_path = Path(self.local_root) / self.storage_dir / Path(path).name
+        md5 = hashlib.md5()
+        with open(path, "rb") as f:
+            for chunk in iter(lambda: f.read(4096), b""):
+                md5.update(chunk)
+        filename = f"{md5.hexdigest()}{''.join(Path(path).suffixes)}"
+        local_path = Path(self.local_root) / self.storage_dir / filename
         local_path.parent.mkdir(parents=True, exist_ok=True)
         with open(path, "rb") as f_in, open(local_path, "wb") as f_out:
             shutil.copyfileobj(f_in, f_out)
         return str(local_path)
```

### Comparing `dwave_sona_core-0.2.8/sona/core/storages/s3.py` & `dwave_sona_core-0.2.9/sona/core/storages/s3.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/inferencers/base.py` & `dwave_sona_core-0.2.9/sona/inferencers/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/inferencers/mock.py` & `dwave_sona_core-0.2.9/sona/inferencers/mock.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/settings.py` & `dwave_sona_core-0.2.9/sona/settings.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/workers/base.py` & `dwave_sona_core-0.2.9/sona/workers/base.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/sona/workers/inferencer.py` & `dwave_sona_core-0.2.9/sona/workers/inferencer.py`

 * *Files identical despite different names*

### Comparing `dwave_sona_core-0.2.8/PKG-INFO` & `dwave_sona_core-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-sona-core
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: dwave-dev
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

