# Comparing `tmp/zlgsendcan-1.0.9.tar.gz` & `tmp/zlgsendcan-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.0.9.tar", last modified: Wed Jul 26 08:14:53 2023, max compression
+gzip compressed data, was "zlgsendcan-1.1.0.tar", last modified: Wed Jul 26 08:41:15 2023, max compression
```

## Comparing `zlgsendcan-1.0.9.tar` & `zlgsendcan-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:14:53.325880 zlgsendcan-1.0.9/
--rw-rw-rw-   0        0        0      220 2023-07-26 08:14:53.324880 zlgsendcan-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 08:14:53.325880 zlgsendcan-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      455 2023-07-26 08:14:31.000000 zlgsendcan-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:14:53.317396 zlgsendcan-1.0.9/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.0.9/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.0.9/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     2995 2023-07-26 06:37:07.000000 zlgsendcan-1.0.9/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.0.9/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1121 2023-01-28 01:59:44.000000 zlgsendcan-1.0.9/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    24969 2023-07-26 06:37:07.000000 zlgsendcan-1.0.9/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.0.9/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:14:53.323881 zlgsendcan-1.0.9/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-26 08:14:53.000000 zlgsendcan-1.0.9/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-26 08:14:53.000000 zlgsendcan-1.0.9/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 08:14:53.000000 zlgsendcan-1.0.9/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 08:14:53.000000 zlgsendcan-1.0.9/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 08:14:53.000000 zlgsendcan-1.0.9/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:15.942675 zlgsendcan-1.1.0/
+-rw-rw-rw-   0        0        0      220 2023-07-26 08:41:15.941675 zlgsendcan-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:41:15.942675 zlgsendcan-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      455 2023-07-26 08:41:10.000000 zlgsendcan-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:15.933674 zlgsendcan-1.1.0/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.0/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.0/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3011 2023-07-26 08:41:01.000000 zlgsendcan-1.1.0/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.1.0/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.0/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    24969 2023-07-26 06:37:07.000000 zlgsendcan-1.1.0/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.1.0/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:15.940676 zlgsendcan-1.1.0/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-26 08:41:15.000000 zlgsendcan-1.1.0/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-26 08:41:15.000000 zlgsendcan-1.1.0/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:41:15.000000 zlgsendcan-1.1.0/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 08:41:15.000000 zlgsendcan-1.1.0/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 08:41:15.000000 zlgsendcan-1.1.0/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.0.9/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.1.0/zlgsendcan/get_conf_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 
 from zlgsendcan import frozen_dir
-import yaml_util
+from zlgsendcan import yaml_util
 
 SETUP_DIR = frozen_dir.app_path()
 sys.path.append(SETUP_DIR)
 # 获取当前项目的绝对路径
 # current = os.path.abspath(__file__)
 # base_dir = os.path.dirname(os.path.dirname(current))
 # log路径
```

### Comparing `zlgsendcan-1.0.9/zlgsendcan/parseDBC.py` & `zlgsendcan-1.1.0/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.0.9/zlgsendcan/yaml_util.py` & `zlgsendcan-1.1.0/zlgsendcan/yaml_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,24 +13,22 @@
 
     def read_data(self):
         """
         单个文档读取
         :return:
         """
         if not self._data:
-            with open(self.yaml_file, "r",encoding='utf-8') as f:
+            with open(self.yaml_file, "r", encoding='utf-8') as f:
                 self._data = yaml.safe_load(f)
         return self._data
 
     def read_data_all(self):
         if not self._data_all:
-            with open(self.yaml_file, "r",encoding='utf-8') as f:
+            with open(self.yaml_file, "r", encoding='utf-8') as f:
                 self._data_all = list(yaml.safe_load_all(f))
         return self._data_all
 
-    def updata_yaml(self,old_data):
+    def updata_yaml(self, old_data):
         # old_data = self.read_data()  # 读取文件数据
         # old_data['can初始化配置'][k] = v  # 修改读取的数据（k存在就修改对应值，k不存在就新增一组键值对）
-        with open( self.yaml_file, "w", encoding="utf-8") as f:
-            yaml.dump(old_data, f,allow_unicode=True)
-
-
+        with open(self.yaml_file, "w", encoding="utf-8") as f:
+            yaml.dump(old_data, f, allow_unicode=True)
```

### Comparing `zlgsendcan-1.0.9/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.1.0/zlgsendcan/zlgcan1.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.0.9/zlgsendcan/zlgserver.py` & `zlgsendcan-1.1.0/zlgsendcan/zlgserver.py`

 * *Files identical despite different names*

