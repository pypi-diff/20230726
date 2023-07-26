# Comparing `tmp/EstymaApiWrapper-0.0.53.tar.gz` & `tmp/EstymaApiWrapper-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EstymaApiWrapper-0.0.53.tar", last modified: Tue Apr 26 20:33:28 2022, max compression
+gzip compressed data, was "EstymaApiWrapper-0.0.54.tar", last modified: Wed Jul 26 11:11:54 2023, max compression
```

## Comparing `EstymaApiWrapper-0.0.53.tar` & `EstymaApiWrapper-0.0.54.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 20:33:28.124641 EstymaApiWrapper-0.0.53/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-04-26 20:33:15.000000 EstymaApiWrapper-0.0.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      772 2022-04-26 20:33:28.124641 EstymaApiWrapper-0.0.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      237 2022-04-26 20:33:15.000000 EstymaApiWrapper-0.0.53/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      103 2022-04-26 20:33:15.000000 EstymaApiWrapper-0.0.53/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      686 2022-04-26 20:33:28.124641 EstymaApiWrapper-0.0.53/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 20:33:28.124641 EstymaApiWrapper-0.0.53/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 20:33:28.124641 EstymaApiWrapper-0.0.53/src/EstymaApiWrapper/
--rw-r--r--   0 runner    (1001) docker     (116)     7383 2022-04-26 20:33:15.000000 EstymaApiWrapper-0.0.53/src/EstymaApiWrapper/EstymaApi.py
--rw-r--r--   0 runner    (1001) docker     (116)       32 2022-04-26 20:33:15.000000 EstymaApiWrapper-0.0.53/src/EstymaApiWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3729 2022-04-26 20:33:15.000000 EstymaApiWrapper-0.0.53/src/EstymaApiWrapper/api_translation_table.json
--rw-r--r--   0 runner    (1001) docker     (116)      280 2022-04-26 20:33:15.000000 EstymaApiWrapper-0.0.53/src/EstymaApiWrapper/languageTable.json
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-04-26 20:33:28.124641 EstymaApiWrapper-0.0.53/src/EstymaApiWrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      772 2022-04-26 20:33:27.000000 EstymaApiWrapper-0.0.53/src/EstymaApiWrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      373 2022-04-26 20:33:28.000000 EstymaApiWrapper-0.0.53/src/EstymaApiWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-04-26 20:33:27.000000 EstymaApiWrapper-0.0.53/src/EstymaApiWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2022-04-26 20:33:28.000000 EstymaApiWrapper-0.0.53/src/EstymaApiWrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 11:11:54.466248 EstymaApiWrapper-0.0.54/
+-rw-rw-rw-   0        0        0        0 2023-07-26 10:15:41.000000 EstymaApiWrapper-0.0.54/LICENSE
+-rw-rw-rw-   0        0        0      821 2023-07-26 11:11:54.467265 EstymaApiWrapper-0.0.54/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-07-26 10:15:41.000000 EstymaApiWrapper-0.0.54/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-26 10:15:41.000000 EstymaApiWrapper-0.0.54/pyproject.toml
+-rw-rw-rw-   0        0        0      719 2023-07-26 11:11:54.474541 EstymaApiWrapper-0.0.54/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-07-26 10:32:29.000000 EstymaApiWrapper-0.0.54/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:11:54.419431 EstymaApiWrapper-0.0.54/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 11:11:54.445488 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper/
+-rw-rw-rw-   0        0        0      329 2023-07-26 10:15:41.000000 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper/CustomErrors.py
+-rw-rw-rw-   0        0        0    15903 2023-07-26 11:03:01.000000 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper/EstymaApi.py
+-rw-rw-rw-   0        0        0       32 2023-07-26 10:15:41.000000 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper/__init__.py
+-rw-rw-rw-   0        0        0     4267 2023-07-26 10:15:41.000000 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper/api_translation_table.json
+-rw-rw-rw-   0        0        0      292 2023-07-26 10:15:41.000000 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper/languageTable.json
+drwxrwxrwx   0        0        0        0 2023-07-26 11:11:54.464750 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper.egg-info/
+-rw-rw-rw-   0        0        0      821 2023-07-26 11:11:54.000000 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-07-26 11:11:54.000000 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 11:11:54.000000 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 11:11:54.000000 EstymaApiWrapper-0.0.54/src/EstymaApiWrapper.egg-info/top_level.txt
```

### Comparing `EstymaApiWrapper-0.0.53/PKG-INFO` & `EstymaApiWrapper-0.0.54/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1
-Name: EstymaApiWrapper
-Version: 0.0.53
-Summary: Wrapper for the EstymaApi
-Home-page: https://github.com/Tabisch/EstymaApi
-Author: Tabisch
-Author-email: tobithieman@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/Tabisch/EstymaApi/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Wrapper for the EstymaApi Heating Systems
-
-This is a work in progess and will only include readind stuff from the api.
-Im building this to integrate our heating system into home assistant.
-
-https://github.com/Tabisch/Igneo_ha_integration
-
+Metadata-Version: 2.1
+Name: EstymaApiWrapper
+Version: 0.0.54
+Summary: Wrapper for the EstymaApi
+Home-page: https://github.com/Tabisch/EstymaApi
+Author: Tabisch
+Author-email: tobithieman@gmail.com
+Project-URL: Bug Tracker, https://github.com/Tabisch/EstymaApi/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Wrapper for the EstymaApi Heating Systems
+
+This is a work in progess.
+At the moment the main pupose is reading data.
+Changing settings is working but still in a really early stage.
+Im building this to integrate our heating system into home assistant.
+
+https://github.com/Tabisch/Igneo_ha_integration
```

### Comparing `EstymaApiWrapper-0.0.53/setup.cfg` & `EstymaApiWrapper-0.0.54/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 4573 7479 6d61 4170 6957 7261 7070  = EstymaApiWrapp
-00000020: 6572 0a76 6572 7369 6f6e 203d 2030 2e30  er.version = 0.0
-00000030: 2e35 330a 6175 7468 6f72 203d 2054 6162  .53.author = Tab
-00000040: 6973 6368 0a61 7574 686f 725f 656d 6169  isch.author_emai
-00000050: 6c20 3d20 746f 6269 7468 6965 6d61 6e40  l = tobithieman@
-00000060: 676d 6169 6c2e 636f 6d0a 6465 7363 7269  gmail.com.descri
-00000070: 7074 696f 6e20 3d20 5772 6170 7065 7220  ption = Wrapper 
-00000080: 666f 7220 7468 6520 4573 7479 6d61 4170  for the EstymaAp
-00000090: 690a 6c6f 6e67 5f64 6573 6372 6970 7469  i.long_descripti
-000000a0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
-000000b0: 452e 6d64 0a6c 6f6e 675f 6465 7363 7269  E.md.long_descri
-000000c0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-000000d0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-000000e0: 776e 0a75 726c 203d 2068 7474 7073 3a2f  wn.url = https:/
-000000f0: 2f67 6974 6875 622e 636f 6d2f 5461 6269  /github.com/Tabi
-00000100: 7363 682f 4573 7479 6d61 4170 690a 7072  sch/EstymaApi.pr
-00000110: 6f6a 6563 745f 7572 6c73 203d 200a 0942  oject_urls = ..B
-00000120: 7567 2054 7261 636b 6572 203d 2068 7474  ug Tracker = htt
-00000130: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000140: 5461 6269 7363 682f 4573 7479 6d61 4170  Tabisch/EstymaAp
-00000150: 692f 6973 7375 6573 0a63 6c61 7373 6966  i/issues.classif
-00000160: 6965 7273 203d 200a 0950 726f 6772 616d  iers = ..Program
-00000170: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000180: 2050 7974 686f 6e20 3a3a 2033 0a09 4c69   Python :: 3..Li
-00000190: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-000001a0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-000001b0: 656e 7365 0a09 4f70 6572 6174 696e 6720  ense..Operating 
-000001c0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-000001d0: 6570 656e 6465 6e74 0a0a 5b6f 7074 696f  ependent..[optio
-000001e0: 6e73 5d0a 7061 636b 6167 655f 6469 7220  ns].package_dir 
-000001f0: 3d20 0a09 3d20 7372 630a 7061 636b 6167  = ..= src.packag
-00000200: 6573 203d 2066 696e 643a 0a70 7974 686f  es = find:.pytho
-00000210: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000220: 2e39 0a69 6e63 6c75 6465 5f70 6163 6b61  .9.include_packa
-00000230: 6765 5f64 6174 6120 3d20 5472 7565 0a0a  ge_data = True..
-00000240: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000250: 732e 6669 6e64 5d0a 7768 6572 6520 3d20  s.find].where = 
-00000260: 7372 630a 0a5b 6f70 7469 6f6e 732e 7061  src..[options.pa
-00000270: 636b 6167 655f 6461 7461 5d0a 2a20 3d20  ckage_data].* = 
-00000280: 2a2e 6a73 6f6e 0a0a 5b65 6767 5f69 6e66  *.json..[egg_inf
-00000290: 6f5d 0a74 6167 5f62 7569 6c64 203d 200a  o].tag_build = .
-000002a0: 7461 675f 6461 7465 203d 2030 0a0a       tag_date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2045 7374 796d 6141 7069 5772 6170   = EstymaApiWrap
+00000020: 7065 720d 0a76 6572 7369 6f6e 203d 2030  per..version = 0
+00000030: 2e30 2e35 340d 0a61 7574 686f 7220 3d20  .0.54..author = 
+00000040: 5461 6269 7363 680d 0a61 7574 686f 725f  Tabisch..author_
+00000050: 656d 6169 6c20 3d20 746f 6269 7468 6965  email = tobithie
+00000060: 6d61 6e40 676d 6169 6c2e 636f 6d0d 0a64  man@gmail.com..d
+00000070: 6573 6372 6970 7469 6f6e 203d 2057 7261  escription = Wra
+00000080: 7070 6572 2066 6f72 2074 6865 2045 7374  pper for the Est
+00000090: 796d 6141 7069 0d0a 6c6f 6e67 5f64 6573  ymaApi..long_des
+000000a0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000b0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
+000000c0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+000000d0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+000000e0: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
+000000f0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000100: 636f 6d2f 5461 6269 7363 682f 4573 7479  com/Tabisch/Esty
+00000110: 6d61 4170 690d 0a70 726f 6a65 6374 5f75  maApi..project_u
+00000120: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
+00000130: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
+00000140: 6974 6875 622e 636f 6d2f 5461 6269 7363  ithub.com/Tabisc
+00000150: 682f 4573 7479 6d61 4170 692f 6973 7375  h/EstymaApi/issu
+00000160: 6573 0d0a 636c 6173 7369 6669 6572 7320  es..classifiers 
+00000170: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
+00000180: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000190: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
+000001a0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+000001b0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+000001c0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
+000001d0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+000001e0: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
+000001f0: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+00000200: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
+00000210: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
+00000220: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+00000230: 203e 3d33 2e39 0d0a 696e 636c 7564 655f   >=3.9..include_
+00000240: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
+00000250: 7275 650d 0a0d 0a5b 6f70 7469 6f6e 732e  rue....[options.
+00000260: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000270: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+00000280: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
+00000290: 6461 7461 5d0d 0a2a 203d 202a 2e6a 736f  data]..* = *.jso
+000002a0: 6e0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  n....[egg_info].
+000002b0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+000002c0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `EstymaApiWrapper-0.0.53/src/EstymaApiWrapper.egg-info/PKG-INFO` & `EstymaApiWrapper-0.0.54/src/EstymaApiWrapper.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1
-Name: EstymaApiWrapper
-Version: 0.0.53
-Summary: Wrapper for the EstymaApi
-Home-page: https://github.com/Tabisch/EstymaApi
-Author: Tabisch
-Author-email: tobithieman@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/Tabisch/EstymaApi/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-Wrapper for the EstymaApi Heating Systems
-
-This is a work in progess and will only include readind stuff from the api.
-Im building this to integrate our heating system into home assistant.
-
-https://github.com/Tabisch/Igneo_ha_integration
-
+Metadata-Version: 2.1
+Name: EstymaApiWrapper
+Version: 0.0.54
+Summary: Wrapper for the EstymaApi
+Home-page: https://github.com/Tabisch/EstymaApi
+Author: Tabisch
+Author-email: tobithieman@gmail.com
+Project-URL: Bug Tracker, https://github.com/Tabisch/EstymaApi/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Wrapper for the EstymaApi Heating Systems
+
+This is a work in progess.
+At the moment the main pupose is reading data.
+Changing settings is working but still in a really early stage.
+Im building this to integrate our heating system into home assistant.
+
+https://github.com/Tabisch/Igneo_ha_integration
```

