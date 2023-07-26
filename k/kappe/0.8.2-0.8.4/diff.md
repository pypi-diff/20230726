# Comparing `tmp/kappe-0.8.2.tar.gz` & `tmp/kappe-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappe-0.8.2.tar", last modified: Thu Jul 20 15:27:06 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `kappe-0.8.2.tar` & `kappe-0.8.4.tar`

### file list

```diff
@@ -1,37 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 15:26:53.000000 kappe-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 15:27:06.506395 kappe-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 15:26:53.000000 kappe-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-20 15:26:53.000000 kappe-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:27:06.506395 kappe-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.502395 kappe-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/src/kappe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/kappe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/src/kappe/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/module/pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/module/qos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/module/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/module/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/src/kappe/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/src/kappe/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/utils/msg_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/utils/pointcloud2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-20 15:26:53.000000 kappe-0.8.2/src/kappe/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:27:06.506395 kappe-0.8.2/src/kappe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 15:27:06.000000 kappe-0.8.2/src/kappe.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 kappe-0.8.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 kappe-0.8.4/.python-version
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 kappe-0.8.4/CHANGELOG.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kappe-0.8.4/MANIFEST.in
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kappe-0.8.4/committed.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kappe-0.8.4/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/__main__.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/cli.py
+-rw-r--r--   0        0        0    15660 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/convert.py
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/cut.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/plugin.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/module/__init__.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/module/pointcloud.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/module/qos.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/module/tf.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/module/timing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/plugins/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/plugins/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/utils/__init__.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/utils/msg_def.py
+-rw-r--r--   0        0        0     8318 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/utils/pointcloud2.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/utils/settings.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 kappe-0.8.4/src/kappe/utils/types.py
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 kappe-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 kappe-0.8.4/LICENSE
+-rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 kappe-0.8.4/README.md
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 kappe-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 kappe-0.8.4/PKG-INFO
```

### Comparing `kappe-0.8.2/src/kappe/convert.py` & `kappe-0.8.4/src/kappe/convert.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.2/src/kappe/cut.py` & `kappe-0.8.4/src/kappe/cut.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from pydantic import BaseModel, Extra, Field, validator
 from tqdm import tqdm
 
 logger = logging.getLogger(__name__)
 
 
 class CutSplits(BaseModel, extra=Extra.forbid):
-    # TODO: validate that start is >= file start
-    # TODO: validate that end is <= file end
     start: float
     end: float
     name: str
 
     @validator('end')
     def validate_end(cls, value, values, **kwargs):  # noqa: ANN001, ANN003, ANN201, ARG003
         if value < values['start']:
```

### Comparing `kappe-0.8.2/src/kappe/kappe.py` & `kappe-0.8.4/src/kappe/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         '--overwrite',
         action='store_true',
         help='Overwrite existing files')
 
     convert = sub.add_parser('convert')
     convert.set_defaults(func=cmd_convert)
 
-    convert.add_argument('input', type=Path, help='input folder')
+    convert.add_argument('input', type=Path, help='input folder or file')
     convert.add_argument('output', type=Path, help='output folder')
     convert.add_argument('--config', type=argparse.FileType(), help='config file')
     convert.add_argument(
         '--overwrite',
         action='store_true',
         help='Overwrite existing files')
```

### Comparing `kappe-0.8.2/src/kappe/module/pointcloud.py` & `kappe-0.8.4/src/kappe/module/pointcloud.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.2/src/kappe/module/qos.py` & `kappe-0.8.4/src/kappe/module/qos.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.2/src/kappe/module/tf.py` & `kappe-0.8.4/src/kappe/module/tf.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.2/src/kappe/module/timing.py` & `kappe-0.8.4/src/kappe/module/timing.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.2/src/kappe/plugin.py` & `kappe-0.8.4/src/kappe/plugin.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.2/src/kappe/plugins/image.py` & `kappe-0.8.4/src/kappe/plugins/image.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.2/src/kappe/settings.py` & `kappe-0.8.4/src/kappe/settings.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.2/src/kappe/utils/msg_def.py` & `kappe-0.8.4/src/kappe/utils/msg_def.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.2/src/kappe/utils/pointcloud2.py` & `kappe-0.8.4/src/kappe/utils/pointcloud2.py`

 * *Files identical despite different names*

### Comparing `kappe-0.8.2/src/kappe/utils/settings.py` & `kappe-0.8.4/src/kappe/utils/settings.py`

 * *Files identical despite different names*

