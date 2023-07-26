# Comparing `tmp/max_util-0.0.4.tar.gz` & `tmp/max_util-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "max_util-0.0.4.tar", last modified: Tue Jul 25 14:10:42 2023, max compression
+gzip compressed data, was "max_util-0.0.6.tar", last modified: Wed Jul 26 13:15:18 2023, max compression
```

## Comparing `max_util-0.0.4.tar` & `max_util-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:42.788357 max_util-0.0.4/
--rw-rw-rw-   0        0        0     1091 2021-10-29 14:52:05.000000 max_util-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      707 2023-07-25 14:10:42.789356 max_util-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      196 2021-11-04 16:24:29.000000 max_util-0.0.4/README.md
--rw-rw-rw-   0        0        0      122 2021-12-25 16:29:55.000000 max_util-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      646 2023-07-25 14:10:42.791350 max_util-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:42.690618 max_util-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:42.703585 max_util-0.0.4/src/alios/
--rw-rw-rw-   0        0        0        0 2023-07-19 13:14:48.000000 max_util-0.0.4/src/alios/__init__.py
--rw-rw-rw-   0        0        0     1169 2023-07-25 14:01:10.000000 max_util-0.0.4/src/alios/api.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:42.719541 max_util-0.0.4/src/excel_util/
--rw-rw-rw-   0        0        0       30 2021-10-29 16:15:34.000000 max_util-0.0.4/src/excel_util/__init__.py
--rw-rw-rw-   0        0        0     1778 2022-07-05 13:29:05.000000 max_util-0.0.4/src/excel_util/mk_book.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:42.735499 max_util-0.0.4/src/max_util.egg-info/
--rw-rw-rw-   0        0        0      707 2023-07-25 14:10:42.000000 max_util-0.0.4/src/max_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-25 14:10:42.000000 max_util-0.0.4/src/max_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:10:42.000000 max_util-0.0.4/src/max_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-25 14:10:42.000000 max_util-0.0.4/src/max_util.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:42.752574 max_util-0.0.4/src/setting/
--rw-rw-rw-   0        0        0        0 2023-07-18 14:21:25.000000 max_util-0.0.4/src/setting/__init__.py
--rw-rw-rw-   0        0        0     1181 2023-07-18 14:22:15.000000 max_util-0.0.4/src/setting/json_config.py
--rw-rw-rw-   0        0        0      350 2023-07-17 14:10:08.000000 max_util-0.0.4/src/setting/util.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:42.772401 max_util-0.0.4/src/showdoc/
--rw-rw-rw-   0        0        0     3773 2023-07-25 14:02:59.000000 max_util-0.0.4/src/showdoc/__init__.py
--rw-rw-rw-   0        0        0     3779 2023-07-19 16:06:18.000000 max_util-0.0.4/src/showdoc/api.py
--rw-rw-rw-   0        0        0     2102 2023-07-20 14:10:25.000000 max_util-0.0.4/src/showdoc/entity.py
--rw-rw-rw-   0        0        0     2728 2023-07-25 13:59:48.000000 max_util-0.0.4/src/showdoc/util.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:42.787360 max_util-0.0.4/src/turtle_util/
--rw-rw-rw-   0        0        0       23 2021-12-25 16:26:06.000000 max_util-0.0.4/src/turtle_util/__init__.py
--rw-rw-rw-   0        0        0     7989 2021-12-25 16:26:06.000000 max_util-0.0.4/src/turtle_util/christmas_2021.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:15:18.869829 max_util-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2021-10-29 14:52:05.000000 max_util-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      707 2023-07-26 13:15:18.869829 max_util-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2021-11-04 16:24:29.000000 max_util-0.0.6/README.md
+-rw-rw-rw-   0        0        0      122 2021-12-25 16:29:55.000000 max_util-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      646 2023-07-26 13:15:18.871824 max_util-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 13:15:18.830907 max_util-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 13:15:18.838849 max_util-0.0.6/src/alios/
+-rw-rw-rw-   0        0        0       10 2023-07-26 13:10:36.000000 max_util-0.0.6/src/alios/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-07-26 13:10:13.000000 max_util-0.0.6/src/alios/api.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:15:18.840844 max_util-0.0.6/src/excel_util/
+-rw-rw-rw-   0        0        0       30 2021-10-29 16:15:34.000000 max_util-0.0.6/src/excel_util/__init__.py
+-rw-rw-rw-   0        0        0     1778 2022-07-05 13:29:05.000000 max_util-0.0.6/src/excel_util/mk_book.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:15:18.856580 max_util-0.0.6/src/max_util.egg-info/
+-rw-rw-rw-   0        0        0      707 2023-07-26 13:15:18.000000 max_util-0.0.6/src/max_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-26 13:15:18.000000 max_util-0.0.6/src/max_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 13:15:18.000000 max_util-0.0.6/src/max_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-26 13:15:18.000000 max_util-0.0.6/src/max_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 13:15:18.861913 max_util-0.0.6/src/setting/
+-rw-rw-rw-   0        0        0      150 2023-07-26 13:12:58.000000 max_util-0.0.6/src/setting/__init__.py
+-rw-rw-rw-   0        0        0     1181 2023-07-18 14:22:15.000000 max_util-0.0.6/src/setting/json_config.py
+-rw-rw-rw-   0        0        0      350 2023-07-17 14:10:08.000000 max_util-0.0.6/src/setting/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:15:18.865841 max_util-0.0.6/src/showdoc/
+-rw-rw-rw-   0        0        0     3843 2023-07-26 13:14:40.000000 max_util-0.0.6/src/showdoc/__init__.py
+-rw-rw-rw-   0        0        0     3781 2023-07-26 13:00:44.000000 max_util-0.0.6/src/showdoc/api.py
+-rw-rw-rw-   0        0        0     2102 2023-07-20 14:10:25.000000 max_util-0.0.6/src/showdoc/entity.py
+-rw-rw-rw-   0        0        0     2728 2023-07-25 13:59:48.000000 max_util-0.0.6/src/showdoc/util.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:15:18.868833 max_util-0.0.6/src/turtle_util/
+-rw-rw-rw-   0        0        0       23 2021-12-25 16:26:06.000000 max_util-0.0.6/src/turtle_util/__init__.py
+-rw-rw-rw-   0        0        0     7989 2021-12-25 16:26:06.000000 max_util-0.0.6/src/turtle_util/christmas_2021.py
```

### Comparing `max_util-0.0.4/LICENSE` & `max_util-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `max_util-0.0.4/PKG-INFO` & `max_util-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 206d 6178  : 2.1..Name: max
 00000020: 5f75 7469 6c0d 0a56 6572 7369 6f6e 3a20  _util..Version: 
-00000030: 302e 302e 340d 0a53 756d 6d61 7279 3a20  0.0.4..Summary: 
+00000030: 302e 302e 360d 0a53 756d 6d61 7279 3a20  0.0.6..Summary: 
 00000040: 696e 7365 7274 2065 7863 656c 2062 6f6f  insert excel boo
 00000050: 6b2c 2062 6173 6520 786c 7774 0d0a 486f  k, base xlwt..Ho
 00000060: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000070: 2f67 6974 6565 2e63 6f6d 2f6d 6178 696e  /gitee.com/maxin
 00000080: 787a 2f6d 6b5f 7574 696c 5f70 7974 686f  xz/mk_util_pytho
 00000090: 6e0d 0a41 7574 686f 723a 206d 6178 0d0a  n..Author: max..
 000000a0: 4175 7468 6f72 2d65 6d61 696c 3a20 6d61  Author-email: ma
```

### Comparing `max_util-0.0.4/setup.cfg` & `max_util-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6178 5f75 7469 6c0d 0a76 6572   = max_util..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e34 0d0a 6175  sion = 0.0.4..au
+00000020: 7369 6f6e 203d 2030 2e30 2e36 0d0a 6175  sion = 0.0.6..au
 00000030: 7468 6f72 203d 206d 6178 0d0a 6175 7468  thor = max..auth
 00000040: 6f72 5f65 6d61 696c 203d 206d 615f 6b65  or_email = ma_ke
 00000050: 5f6d 696e 4031 3633 2e63 6f6d 0d0a 6465  _min@163.com..de
 00000060: 7363 7269 7074 696f 6e20 3d20 696e 7365  scription = inse
 00000070: 7274 2065 7863 656c 2062 6f6f 6b2c 2062  rt excel book, b
 00000080: 6173 6520 786c 7774 0d0a 6c6f 6e67 5f64  ase xlwt..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `max_util-0.0.4/src/alios/api.py` & `max_util-0.0.6/src/alios/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import oss2
 from oss2 import Auth, Bucket
 
-from setting.json_config import JsonConf
+from ..setting.json_config import JsonConf
 
 conf_url = '.aliOSS/conf.json'
 
 
 class API:
     __access_key: str
     __access_secret: str
```

### Comparing `max_util-0.0.4/src/excel_util/mk_book.py` & `max_util-0.0.6/src/excel_util/mk_book.py`

 * *Files identical despite different names*

### Comparing `max_util-0.0.4/src/max_util.egg-info/PKG-INFO` & `max_util-0.0.6/src/max_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 206d 6178  : 2.1..Name: max
 00000020: 2d75 7469 6c0d 0a56 6572 7369 6f6e 3a20  -util..Version: 
-00000030: 302e 302e 340d 0a53 756d 6d61 7279 3a20  0.0.4..Summary: 
+00000030: 302e 302e 360d 0a53 756d 6d61 7279 3a20  0.0.6..Summary: 
 00000040: 696e 7365 7274 2065 7863 656c 2062 6f6f  insert excel boo
 00000050: 6b2c 2062 6173 6520 786c 7774 0d0a 486f  k, base xlwt..Ho
 00000060: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000070: 2f67 6974 6565 2e63 6f6d 2f6d 6178 696e  /gitee.com/maxin
 00000080: 787a 2f6d 6b5f 7574 696c 5f70 7974 686f  xz/mk_util_pytho
 00000090: 6e0d 0a41 7574 686f 723a 206d 6178 0d0a  n..Author: max..
 000000a0: 4175 7468 6f72 2d65 6d61 696c 3a20 6d61  Author-email: ma
```

### Comparing `max_util-0.0.4/src/setting/json_config.py` & `max_util-0.0.6/src/setting/json_config.py`

 * *Files identical despite different names*

### Comparing `max_util-0.0.4/src/showdoc/__init__.py` & `max_util-0.0.6/src/showdoc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 import time
 
-from . import util
-from . import api
-from . import entity
-from setting.json_config import JsonConf
+# from . import util
+# from . import api
+# from . import entity
+
+import util
+import api
+import entity
+
+from .. import alios
+from ..setting.json_config import JsonConf
+
 API = api.API
+aliapi = alios.api
 save = util.create_dir
 
-import alios.api as aliapi
+
 
 def init(root_url='https://source.showdoc.com.cn/server/index.php?s='):
     print('input your ali access_key:')
     access_key = input()
     print('input your ali access_secret:')
     access_secret = input()
     print('input your ali bucket:')
```

### Comparing `max_util-0.0.4/src/showdoc/api.py` & `max_util-0.0.6/src/showdoc/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 from . import entity
-from setting.json_config import JsonConf
+from ..setting.json_config import JsonConf
 
 conf_url = '.showDoc/conf.json'
 
 class API:
     __conf_url: str
     __root_url: str
     __api_key: str
```

### Comparing `max_util-0.0.4/src/showdoc/entity.py` & `max_util-0.0.6/src/showdoc/entity.py`

 * *Files identical despite different names*

### Comparing `max_util-0.0.4/src/showdoc/util.py` & `max_util-0.0.6/src/showdoc/util.py`

 * *Files identical despite different names*

### Comparing `max_util-0.0.4/src/turtle_util/christmas_2021.py` & `max_util-0.0.6/src/turtle_util/christmas_2021.py`

 * *Files identical despite different names*

