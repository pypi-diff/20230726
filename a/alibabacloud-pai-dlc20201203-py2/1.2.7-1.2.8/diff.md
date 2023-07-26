# Comparing `tmp/alibabacloud_pai-dlc20201203_py2-1.2.7.tar.gz` & `tmp/alibabacloud_pai-dlc20201203_py2-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pai-dlc20201203_py2-1.2.7.tar", last modified: Fri Jul 21 13:05:55 2023, max compression
+gzip compressed data, was "dist/alibabacloud_pai-dlc20201203_py2-1.2.8.tar", last modified: Wed Jul 26 11:30:46 2023, max compression
```

## Comparing `alibabacloud_pai-dlc20201203_py2-1.2.7.tar` & `alibabacloud_pai-dlc20201203_py2-1.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/
--rw-r--r--   0 root         (0) root         (0)      735 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34644 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203/client.py
--rw-r--r--   0 root         (0) root         (0)   199076 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2925 2023-07-21 13:05:55.000000 alibabacloud_pai-dlc20201203_py2-1.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/
+-rw-r--r--   0 root         (0) root         (0)      798 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35880 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203/client.py
+-rw-r--r--   0 root         (0) root         (0)   202346 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-07-26 11:30:46.000000 alibabacloud_pai-dlc20201203_py2-1.2.8/setup.py
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.7/ChangeLog.md` & `alibabacloud_pai-dlc20201203_py2-1.2.8/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-21 Version: 1.2.7
+- Change the API -- GetWebTerminal.
+
 2023-07-19 Version: 1.2.6
 - Open the API.
 
 2023-05-26 Version: 1.2.5
 - Add parameter in JobElasticSpec.
 
 2023-03-23 Version: 1.2.4
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.7/LICENSE` & `alibabacloud_pai-dlc20201203_py2-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.7/PKG-INFO` & `alibabacloud_pai-dlc20201203_py2-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pai-dlc20201203_py2
-Version: 1.2.7
+Version: 1.2.8
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.7/README-CN.md` & `alibabacloud_pai-dlc20201203_py2-1.2.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.7/README.md` & `alibabacloud_pai-dlc20201203_py2-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203/client.py` & `alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,14 +466,48 @@
         )
 
     def get_tensorboard(self, tensorboard_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_tensorboard_with_options(tensorboard_id, request, headers, runtime)
 
+    def get_token_with_options(self, request, headers, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.expire_time):
+            query['ExpireTime'] = request.expire_time
+        if not UtilClient.is_unset(request.target_id):
+            query['TargetId'] = request.target_id
+        if not UtilClient.is_unset(request.target_type):
+            query['TargetType'] = request.target_type
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetToken',
+            version='2020-12-03',
+            protocol='HTTPS',
+            pathname='/api/v1/tokens',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_dlc_20201203_models.GetTokenResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_token(self, request):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_token_with_options(request, headers, runtime)
+
     def get_web_terminal_with_options(self, job_id, pod_id, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.pod_uid):
             query['PodUid'] = request.pod_uid
         req = open_api_models.OpenApiRequest(
             headers=headers,
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203/models.py` & `alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9913,2531 +9913,2735 @@
 00026b80: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
 00026b90: 705f 6d6f 6465 6c20 3d20 5465 6e73 6f72  p_model = Tensor
 00026ba0: 626f 6172 6428 290a 2020 2020 2020 2020  board().        
 00026bb0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
 00026bc0: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
 00026bd0: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
 00026be0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00026bf0: 6c66 0a0a 0a63 6c61 7373 2047 6574 5765  lf...class GetWe
-00026c00: 6254 6572 6d69 6e61 6c52 6571 7565 7374  bTerminalRequest
-00026c10: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-00026c20: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00026c30: 662c 2070 6f64 5f75 6964 3d4e 6f6e 6529  f, pod_uid=None)
-00026c40: 3a0a 2020 2020 2020 2020 2320 506f 6420  :.        # Pod 
-00026c50: 5549 44e3 8082 0a20 2020 2020 2020 2073  UID....        s
-00026c60: 656c 662e 706f 645f 7569 6420 3d20 706f  elf.pod_uid = po
-00026c70: 645f 7569 6420 2023 2074 7970 653a 2073  d_uid  # type: s
-00026c80: 7472 0a0a 2020 2020 6465 6620 7661 6c69  tr..    def vali
-00026c90: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00026ca0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-00026cb0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00026cc0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00026cd0: 7570 6572 2847 6574 5765 6254 6572 6d69  uper(GetWebTermi
-00026ce0: 6e61 6c52 6571 7565 7374 2c20 7365 6c66  nalRequest, self
-00026cf0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00026d00: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00026d10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00026d20: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00026d30: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00026d40: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00026d50: 2069 6620 7365 6c66 2e70 6f64 5f75 6964   if self.pod_uid
-00026d60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00026d70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00026d80: 5b27 506f 6455 6964 275d 203d 2073 656c  ['PodUid'] = sel
-00026d90: 662e 706f 645f 7569 640a 2020 2020 2020  f.pod_uid.      
-00026da0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00026db0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00026dc0: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-00026dd0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00026de0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-00026df0: 2069 6620 6d2e 6765 7428 2750 6f64 5569   if m.get('PodUi
-00026e00: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00026e10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00026e20: 662e 706f 645f 7569 6420 3d20 6d2e 6765  f.pod_uid = m.ge
-00026e30: 7428 2750 6f64 5569 6427 290a 2020 2020  t('PodUid').    
-00026e40: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00026e50: 0a0a 636c 6173 7320 4765 7457 6562 5465  ..class GetWebTe
-00026e60: 726d 696e 616c 5265 7370 6f6e 7365 426f  rminalResponseBo
-00026e70: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
-00026e80: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00026e90: 656c 662c 2072 6571 7565 7374 5f69 643d  elf, request_id=
-00026ea0: 4e6f 6e65 2c20 7765 625f 7465 726d 696e  None, web_termin
-00026eb0: 616c 5f75 726c 3d4e 6f6e 6529 3a0a 2020  al_url=None):.  
-00026ec0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-00026ed0: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
-00026ee0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-00026ef0: 2020 2020 2020 2020 7365 6c66 2e77 6562          self.web
-00026f00: 5f74 6572 6d69 6e61 6c5f 7572 6c20 3d20  _terminal_url = 
-00026f10: 7765 625f 7465 726d 696e 616c 5f75 726c  web_terminal_url
-00026f20: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
-00026f30: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00026f40: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00026f50: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00026f60: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00026f70: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00026f80: 4765 7457 6562 5465 726d 696e 616c 5265  GetWebTerminalRe
-00026f90: 7370 6f6e 7365 426f 6479 2c20 7365 6c66  sponseBody, self
-00026fa0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00026fb0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00026fc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00026fd0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00026fe0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00026ff0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-00027000: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
-00027010: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00027020: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00027030: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
-00027040: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
-00027050: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-00027060: 6c66 2e77 6562 5f74 6572 6d69 6e61 6c5f  lf.web_terminal_
-00027070: 7572 6c20 6973 206e 6f74 204e 6f6e 653a  url is not None:
-00027080: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00027090: 756c 745b 2757 6562 5465 726d 696e 616c  ult['WebTerminal
-000270a0: 5572 6c27 5d20 3d20 7365 6c66 2e77 6562  Url'] = self.web
-000270b0: 5f74 6572 6d69 6e61 6c5f 7572 6c0a 2020  _terminal_url.  
-000270c0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-000270d0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-000270e0: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
-000270f0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-00027100: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-00027110: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-00027120: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
-00027130: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00027140: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-00027150: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
-00027160: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
-00027170: 2069 6620 6d2e 6765 7428 2757 6562 5465   if m.get('WebTe
-00027180: 726d 696e 616c 5572 6c27 2920 6973 206e  rminalUrl') is n
-00027190: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000271a0: 2020 2020 2073 656c 662e 7765 625f 7465       self.web_te
-000271b0: 726d 696e 616c 5f75 726c 203d 206d 2e67  rminal_url = m.g
-000271c0: 6574 2827 5765 6254 6572 6d69 6e61 6c55  et('WebTerminalU
-000271d0: 726c 2729 0a20 2020 2020 2020 2072 6574  rl').        ret
-000271e0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-000271f0: 2047 6574 5765 6254 6572 6d69 6e61 6c52   GetWebTerminalR
-00027200: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-00027210: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00027220: 745f 5f28 7365 6c66 2c20 6865 6164 6572  t__(self, header
-00027230: 733d 4e6f 6e65 2c20 7374 6174 7573 5f63  s=None, status_c
-00027240: 6f64 653d 4e6f 6e65 2c20 626f 6479 3d4e  ode=None, body=N
-00027250: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-00027260: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
-00027270: 6465 7273 2020 2320 7479 7065 3a20 6469  ders  # type: di
-00027280: 6374 5b73 7472 2c20 7374 725d 0a20 2020  ct[str, str].   
-00027290: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-000272a0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-000272b0: 6f64 6520 2023 2074 7970 653a 2069 6e74  ode  # type: int
-000272c0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-000272d0: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
-000272e0: 653a 2047 6574 5765 6254 6572 6d69 6e61  e: GetWebTermina
-000272f0: 6c52 6573 706f 6e73 6542 6f64 790a 0a20  lResponseBody.. 
-00027300: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00027310: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00027320: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-00027330: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
-00027340: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
-00027350: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-00027360: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-00027370: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
-00027380: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
-00027390: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-000273a0: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-000273b0: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
-000273c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000273d0: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
-000273e0: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
-000273f0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-00027400: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-00027410: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-00027420: 7065 7228 4765 7457 6562 5465 726d 696e  per(GetWebTermin
-00027430: 616c 5265 7370 6f6e 7365 2c20 7365 6c66  alResponse, self
-00027440: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-00027450: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-00027460: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00027470: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-00027480: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00027490: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-000274a0: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-000274b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000274c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000274d0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-000274e0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-000274f0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-00027500: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-00027510: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00027520: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-00027530: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-00027540: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-00027550: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-00027560: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00027570: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-00027580: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-00027590: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-000275a0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-000275b0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-000275c0: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-000275d0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-000275e0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-000275f0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-00027600: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-00027610: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00027620: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-00027630: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-00027640: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00027650: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-00027660: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00027670: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-00027680: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-00027690: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-000276a0: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-000276b0: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-000276c0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-000276d0: 656d 705f 6d6f 6465 6c20 3d20 4765 7457  emp_model = GetW
-000276e0: 6562 5465 726d 696e 616c 5265 7370 6f6e  ebTerminalRespon
-000276f0: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
-00027700: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-00027710: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-00027720: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-00027730: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00027740: 656c 660a 0a0a 636c 6173 7320 4c69 7374  elf...class List
-00027750: 4563 7353 7065 6373 5265 7175 6573 7428  EcsSpecsRequest(
-00027760: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-00027770: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00027780: 2c20 6163 6365 6c65 7261 746f 725f 7479  , accelerator_ty
-00027790: 7065 3d4e 6f6e 652c 206f 7264 6572 3d4e  pe=None, order=N
-000277a0: 6f6e 652c 2070 6167 655f 6e75 6d62 6572  one, page_number
-000277b0: 3d4e 6f6e 652c 2070 6167 655f 7369 7a65  =None, page_size
-000277c0: 3d4e 6f6e 652c 2073 6f72 745f 6279 3d4e  =None, sort_by=N
-000277d0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-000277e0: 6c66 2e61 6363 656c 6572 6174 6f72 5f74  lf.accelerator_t
-000277f0: 7970 6520 3d20 6163 6365 6c65 7261 746f  ype = accelerato
-00027800: 725f 7479 7065 2020 2320 7479 7065 3a20  r_type  # type: 
-00027810: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-00027820: 2e6f 7264 6572 203d 206f 7264 6572 2020  .order = order  
-00027830: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00027840: 2020 2020 7365 6c66 2e70 6167 655f 6e75      self.page_nu
-00027850: 6d62 6572 203d 2070 6167 655f 6e75 6d62  mber = page_numb
-00027860: 6572 2020 2320 7479 7065 3a20 696e 740a  er  # type: int.
-00027870: 2020 2020 2020 2020 7365 6c66 2e70 6167          self.pag
-00027880: 655f 7369 7a65 203d 2070 6167 655f 7369  e_size = page_si
-00027890: 7a65 2020 2320 7479 7065 3a20 696e 740a  ze  # type: int.
-000278a0: 2020 2020 2020 2020 7365 6c66 2e73 6f72          self.sor
-000278b0: 745f 6279 203d 2073 6f72 745f 6279 2020  t_by = sort_by  
-000278c0: 2320 7479 7065 3a20 7374 720a 0a20 2020  # type: str..   
-000278d0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-000278e0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-000278f0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-00027900: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00027910: 205f 6d61 7020 3d20 7375 7065 7228 4c69   _map = super(Li
-00027920: 7374 4563 7353 7065 6373 5265 7175 6573  stEcsSpecsReques
-00027930: 742c 2073 656c 6629 2e74 6f5f 6d61 7028  t, self).to_map(
-00027940: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-00027950: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-00027960: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00027970: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-00027980: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-00027990: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000279a0: 6163 6365 6c65 7261 746f 725f 7479 7065  accelerator_type
-000279b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000279c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000279d0: 5b27 4163 6365 6c65 7261 746f 7254 7970  ['AcceleratorTyp
-000279e0: 6527 5d20 3d20 7365 6c66 2e61 6363 656c  e'] = self.accel
-000279f0: 6572 6174 6f72 5f74 7970 650a 2020 2020  erator_type.    
-00027a00: 2020 2020 6966 2073 656c 662e 6f72 6465      if self.orde
-00027a10: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-00027a20: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00027a30: 745b 274f 7264 6572 275d 203d 2073 656c  t['Order'] = sel
-00027a40: 662e 6f72 6465 720a 2020 2020 2020 2020  f.order.        
-00027a50: 6966 2073 656c 662e 7061 6765 5f6e 756d  if self.page_num
-00027a60: 6265 7220 6973 206e 6f74 204e 6f6e 653a  ber is not None:
-00027a70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00027a80: 756c 745b 2750 6167 654e 756d 6265 7227  ult['PageNumber'
-00027a90: 5d20 3d20 7365 6c66 2e70 6167 655f 6e75  ] = self.page_nu
-00027aa0: 6d62 6572 0a20 2020 2020 2020 2069 6620  mber.        if 
-00027ab0: 7365 6c66 2e70 6167 655f 7369 7a65 2069  self.page_size i
-00027ac0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00027ad0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00027ae0: 5061 6765 5369 7a65 275d 203d 2073 656c  PageSize'] = sel
-00027af0: 662e 7061 6765 5f73 697a 650a 2020 2020  f.page_size.    
-00027b00: 2020 2020 6966 2073 656c 662e 736f 7274      if self.sort
-00027b10: 5f62 7920 6973 206e 6f74 204e 6f6e 653a  _by is not None:
-00027b20: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00027b30: 756c 745b 2753 6f72 7442 7927 5d20 3d20  ult['SortBy'] = 
-00027b40: 7365 6c66 2e73 6f72 745f 6279 0a20 2020  self.sort_by.   
-00027b50: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00027b60: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-00027b70: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
-00027b80: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-00027b90: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-00027ba0: 2020 2020 6966 206d 2e67 6574 2827 4163      if m.get('Ac
-00027bb0: 6365 6c65 7261 746f 7254 7970 6527 2920  celeratorType') 
-00027bc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00027bd0: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
-00027be0: 6365 6c65 7261 746f 725f 7479 7065 203d  celerator_type =
-00027bf0: 206d 2e67 6574 2827 4163 6365 6c65 7261   m.get('Accelera
-00027c00: 746f 7254 7970 6527 290a 2020 2020 2020  torType').      
-00027c10: 2020 6966 206d 2e67 6574 2827 4f72 6465    if m.get('Orde
-00027c20: 7227 2920 6973 206e 6f74 204e 6f6e 653a  r') is not None:
-00027c30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00027c40: 662e 6f72 6465 7220 3d20 6d2e 6765 7428  f.order = m.get(
-00027c50: 274f 7264 6572 2729 0a20 2020 2020 2020  'Order').       
-00027c60: 2069 6620 6d2e 6765 7428 2750 6167 654e   if m.get('PageN
-00027c70: 756d 6265 7227 2920 6973 206e 6f74 204e  umber') is not N
-00027c80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00027c90: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
-00027ca0: 7220 3d20 6d2e 6765 7428 2750 6167 654e  r = m.get('PageN
-00027cb0: 756d 6265 7227 290a 2020 2020 2020 2020  umber').        
-00027cc0: 6966 206d 2e67 6574 2827 5061 6765 5369  if m.get('PageSi
-00027cd0: 7a65 2729 2069 7320 6e6f 7420 4e6f 6e65  ze') is not None
-00027ce0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00027cf0: 6c66 2e70 6167 655f 7369 7a65 203d 206d  lf.page_size = m
-00027d00: 2e67 6574 2827 5061 6765 5369 7a65 2729  .get('PageSize')
-00027d10: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00027d20: 7428 2753 6f72 7442 7927 2920 6973 206e  t('SortBy') is n
-00027d30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00027d40: 2020 2020 2073 656c 662e 736f 7274 5f62       self.sort_b
-00027d50: 7920 3d20 6d2e 6765 7428 2753 6f72 7442  y = m.get('SortB
-00027d60: 7927 290a 2020 2020 2020 2020 7265 7475  y').        retu
-00027d70: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-00027d80: 4c69 7374 4563 7353 7065 6373 5265 7370  ListEcsSpecsResp
-00027d90: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
-00027da0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00027db0: 6974 5f5f 2873 656c 662c 2065 6373 5f73  it__(self, ecs_s
-00027dc0: 7065 6373 3d4e 6f6e 652c 2072 6571 7565  pecs=None, reque
-00027dd0: 7374 5f69 643d 4e6f 6e65 2c20 746f 7461  st_id=None, tota
-00027de0: 6c5f 636f 756e 743d 4e6f 6e65 293a 0a20  l_count=None):. 
-00027df0: 2020 2020 2020 2073 656c 662e 6563 735f         self.ecs_
-00027e00: 7370 6563 7320 3d20 6563 735f 7370 6563  specs = ecs_spec
-00027e10: 7320 2023 2074 7970 653a 206c 6973 745b  s  # type: list[
-00027e20: 4563 7353 7065 635d 0a20 2020 2020 2020  EcsSpec].       
-00027e30: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-00027e40: 203d 2072 6571 7565 7374 5f69 6420 2023   = request_id  #
-00027e50: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-00027e60: 2020 2073 656c 662e 746f 7461 6c5f 636f     self.total_co
-00027e70: 756e 7420 3d20 746f 7461 6c5f 636f 756e  unt = total_coun
-00027e80: 7420 2023 2074 7970 653a 206c 6f6e 670a  t  # type: long.
-00027e90: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00027ea0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00027eb0: 2069 6620 7365 6c66 2e65 6373 5f73 7065   if self.ecs_spe
-00027ec0: 6373 3a0a 2020 2020 2020 2020 2020 2020  cs:.            
-00027ed0: 666f 7220 6b20 696e 2073 656c 662e 6563  for k in self.ec
-00027ee0: 735f 7370 6563 733a 0a20 2020 2020 2020  s_specs:.       
-00027ef0: 2020 2020 2020 2020 2069 6620 6b3a 0a20           if k:. 
-00027f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027f10: 2020 206b 2e76 616c 6964 6174 6528 290a     k.validate().
-00027f20: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00027f30: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00027f40: 6d61 7020 3d20 7375 7065 7228 4c69 7374  map = super(List
-00027f50: 4563 7353 7065 6373 5265 7370 6f6e 7365  EcsSpecsResponse
-00027f60: 426f 6479 2c20 7365 6c66 292e 746f 5f6d  Body, self).to_m
-00027f70: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00027f80: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00027f90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00027fa0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00027fb0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00027fc0: 2829 0a20 2020 2020 2020 2072 6573 756c  ().        resul
-00027fd0: 745b 2745 6373 5370 6563 7327 5d20 3d20  t['EcsSpecs'] = 
-00027fe0: 5b5d 0a20 2020 2020 2020 2069 6620 7365  [].        if se
-00027ff0: 6c66 2e65 6373 5f73 7065 6373 2069 7320  lf.ecs_specs is 
-00028000: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00028010: 2020 2020 2020 666f 7220 6b20 696e 2073        for k in s
-00028020: 656c 662e 6563 735f 7370 6563 733a 0a20  elf.ecs_specs:. 
-00028030: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00028040: 6573 756c 745b 2745 6373 5370 6563 7327  esult['EcsSpecs'
-00028050: 5d2e 6170 7065 6e64 286b 2e74 6f5f 6d61  ].append(k.to_ma
-00028060: 7028 2920 6966 206b 2065 6c73 6520 4e6f  p() if k else No
-00028070: 6e65 290a 2020 2020 2020 2020 6966 2073  ne).        if s
-00028080: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
-00028090: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000280a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000280b0: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
-000280c0: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
-000280d0: 2020 2020 2020 6966 2073 656c 662e 746f        if self.to
-000280e0: 7461 6c5f 636f 756e 7420 6973 206e 6f74  tal_count is not
-000280f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00028100: 2020 2072 6573 756c 745b 2754 6f74 616c     result['Total
-00028110: 436f 756e 7427 5d20 3d20 7365 6c66 2e74  Count'] = self.t
-00028120: 6f74 616c 5f63 6f75 6e74 0a20 2020 2020  otal_count.     
-00028130: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00028140: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-00028150: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
-00028160: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-00028170: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-00028180: 2020 7365 6c66 2e65 6373 5f73 7065 6373    self.ecs_specs
-00028190: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
-000281a0: 206d 2e67 6574 2827 4563 7353 7065 6373   m.get('EcsSpecs
-000281b0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000281c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000281d0: 6b20 696e 206d 2e67 6574 2827 4563 7353  k in m.get('EcsS
-000281e0: 7065 6373 2729 3a0a 2020 2020 2020 2020  pecs'):.        
-000281f0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-00028200: 656c 203d 2045 6373 5370 6563 2829 0a20  el = EcsSpec(). 
-00028210: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00028220: 656c 662e 6563 735f 7370 6563 732e 6170  elf.ecs_specs.ap
-00028230: 7065 6e64 2874 656d 705f 6d6f 6465 6c2e  pend(temp_model.
-00028240: 6672 6f6d 5f6d 6170 286b 2929 0a20 2020  from_map(k)).   
-00028250: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-00028260: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
-00028270: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00028280: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-00028290: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
-000282a0: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
-000282b0: 2069 6620 6d2e 6765 7428 2754 6f74 616c   if m.get('Total
-000282c0: 436f 756e 7427 2920 6973 206e 6f74 204e  Count') is not N
-000282d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000282e0: 2073 656c 662e 746f 7461 6c5f 636f 756e   self.total_coun
-000282f0: 7420 3d20 6d2e 6765 7428 2754 6f74 616c  t = m.get('Total
-00028300: 436f 756e 7427 290a 2020 2020 2020 2020  Count').        
-00028310: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00028320: 6173 7320 4c69 7374 4563 7353 7065 6373  ass ListEcsSpecs
-00028330: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-00028340: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-00028350: 6974 5f5f 2873 656c 662c 2068 6561 6465  it__(self, heade
-00028360: 7273 3d4e 6f6e 652c 2073 7461 7475 735f  rs=None, status_
-00028370: 636f 6465 3d4e 6f6e 652c 2062 6f64 793d  code=None, body=
-00028380: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-00028390: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-000283a0: 6164 6572 7320 2023 2074 7970 653a 2064  aders  # type: d
-000283b0: 6963 745b 7374 722c 2073 7472 5d0a 2020  ict[str, str].  
-000283c0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-000283d0: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-000283e0: 636f 6465 2020 2320 7479 7065 3a20 696e  code  # type: in
-000283f0: 740a 2020 2020 2020 2020 7365 6c66 2e62  t.        self.b
-00028400: 6f64 7920 3d20 626f 6479 2020 2320 7479  ody = body  # ty
-00028410: 7065 3a20 4c69 7374 4563 7353 7065 6373  pe: ListEcsSpecs
-00028420: 5265 7370 6f6e 7365 426f 6479 0a0a 2020  ResponseBody..  
-00028430: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00028440: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-00028450: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-00028460: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
-00028470: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
-00028480: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-00028490: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-000284a0: 662e 7374 6174 7573 5f63 6f64 652c 2027  f.status_code, '
-000284b0: 7374 6174 7573 5f63 6f64 6527 290a 2020  status_code').  
-000284c0: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-000284d0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-000284e0: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
-000284f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00028500: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-00028510: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-00028520: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-00028530: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00028540: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00028550: 6572 284c 6973 7445 6373 5370 6563 7352  er(ListEcsSpecsR
-00028560: 6573 706f 6e73 652c 2073 656c 6629 2e74  esponse, self).t
-00028570: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00028580: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00028590: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000285a0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000285b0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000285c0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000285d0: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-000285e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000285f0: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-00028600: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-00028610: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-00028620: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-00028630: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-00028640: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00028650: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-00028660: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-00028670: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
-00028680: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-00028690: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000286a0: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-000286b0: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-000286c0: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-000286d0: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-000286e0: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-000286f0: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
-00028700: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00028710: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00028720: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-00028730: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00028740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028750: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-00028760: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00028770: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-00028780: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-00028790: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000287a0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-000287b0: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-000287c0: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-000287d0: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-000287e0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000287f0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-00028800: 5f6d 6f64 656c 203d 204c 6973 7445 6373  _model = ListEcs
-00028810: 5370 6563 7352 6573 706f 6e73 6542 6f64  SpecsResponseBod
-00028820: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-00028830: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-00028840: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-00028850: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-00028860: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00028870: 0a63 6c61 7373 204c 6973 744a 6f62 7352  .class ListJobsR
-00028880: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-00028890: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-000288a0: 5f5f 2873 656c 662c 2062 7573 696e 6573  __(self, busines
-000288b0: 735f 7573 6572 5f69 643d 4e6f 6e65 2c20  s_user_id=None, 
-000288c0: 6361 6c6c 6572 3d4e 6f6e 652c 2064 6973  caller=None, dis
-000288d0: 706c 6179 5f6e 616d 653d 4e6f 6e65 2c20  play_name=None, 
-000288e0: 656e 645f 7469 6d65 3d4e 6f6e 652c 0a20  end_time=None,. 
-000288f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028900: 6672 6f6d 5f61 6c6c 5f77 6f72 6b73 7061  from_all_workspa
-00028910: 6365 733d 4e6f 6e65 2c20 6a6f 625f 6964  ces=None, job_id
-00028920: 3d4e 6f6e 652c 206a 6f62 5f74 7970 653d  =None, job_type=
-00028930: 4e6f 6e65 2c20 6f72 6465 723d 4e6f 6e65  None, order=None
-00028940: 2c20 7061 6765 5f6e 756d 6265 723d 4e6f  , page_number=No
-00028950: 6e65 2c20 7061 6765 5f73 697a 653d 4e6f  ne, page_size=No
-00028960: 6e65 2c20 7069 7065 6c69 6e65 5f69 643d  ne, pipeline_id=
-00028970: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00028980: 2020 2020 2020 2072 6573 6f75 7263 655f         resource_
-00028990: 6964 3d4e 6f6e 652c 2073 686f 775f 6f77  id=None, show_ow
-000289a0: 6e3d 4e6f 6e65 2c20 736f 7274 5f62 793d  n=None, sort_by=
-000289b0: 4e6f 6e65 2c20 7374 6172 745f 7469 6d65  None, start_time
-000289c0: 3d4e 6f6e 652c 2073 7461 7475 733d 4e6f  =None, status=No
-000289d0: 6e65 2c20 7461 6773 3d4e 6f6e 652c 2077  ne, tags=None, w
-000289e0: 6f72 6b73 7061 6365 5f69 643d 4e6f 6e65  orkspace_id=None
-000289f0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00028a00: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
-00028a10: 203d 2062 7573 696e 6573 735f 7573 6572   = business_user
-00028a20: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
-00028a30: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
-00028a40: 6c6c 6572 203d 2063 616c 6c65 7220 2023  ller = caller  #
-00028a50: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-00028a60: 2020 2073 656c 662e 6469 7370 6c61 795f     self.display_
-00028a70: 6e61 6d65 203d 2064 6973 706c 6179 5f6e  name = display_n
-00028a80: 616d 6520 2023 2074 7970 653a 2073 7472  ame  # type: str
-00028a90: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-00028aa0: 645f 7469 6d65 203d 2065 6e64 5f74 696d  d_time = end_tim
-00028ab0: 6520 2023 2074 7970 653a 2073 7472 0a20  e  # type: str. 
-00028ac0: 2020 2020 2020 2073 656c 662e 6672 6f6d         self.from
-00028ad0: 5f61 6c6c 5f77 6f72 6b73 7061 6365 7320  _all_workspaces 
-00028ae0: 3d20 6672 6f6d 5f61 6c6c 5f77 6f72 6b73  = from_all_works
-00028af0: 7061 6365 7320 2023 2074 7970 653a 2062  paces  # type: b
-00028b00: 6f6f 6c0a 2020 2020 2020 2020 7365 6c66  ool.        self
-00028b10: 2e6a 6f62 5f69 6420 3d20 6a6f 625f 6964  .job_id = job_id
-00028b20: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-00028b30: 2020 2020 2020 7365 6c66 2e6a 6f62 5f74        self.job_t
-00028b40: 7970 6520 3d20 6a6f 625f 7479 7065 2020  ype = job_type  
-00028b50: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00028b60: 2020 2020 7365 6c66 2e6f 7264 6572 203d      self.order =
-00028b70: 206f 7264 6572 2020 2320 7479 7065 3a20   order  # type: 
-00028b80: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-00028b90: 2e70 6167 655f 6e75 6d62 6572 203d 2070  .page_number = p
-00028ba0: 6167 655f 6e75 6d62 6572 2020 2320 7479  age_number  # ty
-00028bb0: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
-00028bc0: 7365 6c66 2e70 6167 655f 7369 7a65 203d  self.page_size =
-00028bd0: 2070 6167 655f 7369 7a65 2020 2320 7479   page_size  # ty
-00028be0: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
-00028bf0: 7365 6c66 2e70 6970 656c 696e 655f 6964  self.pipeline_id
-00028c00: 203d 2070 6970 656c 696e 655f 6964 2020   = pipeline_id  
-00028c10: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00028c20: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
-00028c30: 655f 6964 203d 2072 6573 6f75 7263 655f  e_id = resource_
-00028c40: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-00028c50: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
-00028c60: 775f 6f77 6e20 3d20 7368 6f77 5f6f 776e  w_own = show_own
-00028c70: 2020 2320 7479 7065 3a20 626f 6f6c 0a20    # type: bool. 
-00028c80: 2020 2020 2020 2073 656c 662e 736f 7274         self.sort
-00028c90: 5f62 7920 3d20 736f 7274 5f62 7920 2023  _by = sort_by  #
-00028ca0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-00028cb0: 2020 2073 656c 662e 7374 6172 745f 7469     self.start_ti
-00028cc0: 6d65 203d 2073 7461 7274 5f74 696d 6520  me = start_time 
-00028cd0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-00028ce0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00028cf0: 203d 2073 7461 7475 7320 2023 2074 7970   = status  # typ
-00028d00: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-00028d10: 656c 662e 7461 6773 203d 2074 6167 7320  elf.tags = tags 
-00028d20: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
-00028d30: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
-00028d40: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
-00028d50: 6420 3d20 776f 726b 7370 6163 655f 6964  d = workspace_id
-00028d60: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
-00028d70: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-00028d80: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00028d90: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-00028da0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-00028db0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-00028dc0: 4c69 7374 4a6f 6273 5265 7175 6573 742c  ListJobsRequest,
-00028dd0: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-00028de0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00028df0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00028e00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00028e10: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00028e20: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00028e30: 2020 2020 2020 6966 2073 656c 662e 6275        if self.bu
-00028e40: 7369 6e65 7373 5f75 7365 725f 6964 2069  siness_user_id i
-00028e50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00028e60: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00028e70: 4275 7369 6e65 7373 5573 6572 4964 275d  BusinessUserId']
-00028e80: 203d 2073 656c 662e 6275 7369 6e65 7373   = self.business
-00028e90: 5f75 7365 725f 6964 0a20 2020 2020 2020  _user_id.       
-00028ea0: 2069 6620 7365 6c66 2e63 616c 6c65 7220   if self.caller 
-00028eb0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00028ec0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00028ed0: 2743 616c 6c65 7227 5d20 3d20 7365 6c66  'Caller'] = self
-00028ee0: 2e63 616c 6c65 720a 2020 2020 2020 2020  .caller.        
-00028ef0: 6966 2073 656c 662e 6469 7370 6c61 795f  if self.display_
-00028f00: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-00028f10: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00028f20: 7375 6c74 5b27 4469 7370 6c61 794e 616d  sult['DisplayNam
-00028f30: 6527 5d20 3d20 7365 6c66 2e64 6973 706c  e'] = self.displ
-00028f40: 6179 5f6e 616d 650a 2020 2020 2020 2020  ay_name.        
-00028f50: 6966 2073 656c 662e 656e 645f 7469 6d65  if self.end_time
-00028f60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028f70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00028f80: 5b27 456e 6454 696d 6527 5d20 3d20 7365  ['EndTime'] = se
-00028f90: 6c66 2e65 6e64 5f74 696d 650a 2020 2020  lf.end_time.    
-00028fa0: 2020 2020 6966 2073 656c 662e 6672 6f6d      if self.from
-00028fb0: 5f61 6c6c 5f77 6f72 6b73 7061 6365 7320  _all_workspaces 
-00028fc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00028fd0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00028fe0: 2746 726f 6d41 6c6c 576f 726b 7370 6163  'FromAllWorkspac
-00028ff0: 6573 275d 203d 2073 656c 662e 6672 6f6d  es'] = self.from
-00029000: 5f61 6c6c 5f77 6f72 6b73 7061 6365 730a  _all_workspaces.
-00029010: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00029020: 6a6f 625f 6964 2069 7320 6e6f 7420 4e6f  job_id is not No
-00029030: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00029040: 7265 7375 6c74 5b27 4a6f 6249 6427 5d20  result['JobId'] 
-00029050: 3d20 7365 6c66 2e6a 6f62 5f69 640a 2020  = self.job_id.  
-00029060: 2020 2020 2020 6966 2073 656c 662e 6a6f        if self.jo
-00029070: 625f 7479 7065 2069 7320 6e6f 7420 4e6f  b_type is not No
-00029080: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00029090: 7265 7375 6c74 5b27 4a6f 6254 7970 6527  result['JobType'
-000290a0: 5d20 3d20 7365 6c66 2e6a 6f62 5f74 7970  ] = self.job_typ
-000290b0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-000290c0: 662e 6f72 6465 7220 6973 206e 6f74 204e  f.order is not N
-000290d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000290e0: 2072 6573 756c 745b 274f 7264 6572 275d   result['Order']
-000290f0: 203d 2073 656c 662e 6f72 6465 720a 2020   = self.order.  
-00029100: 2020 2020 2020 6966 2073 656c 662e 7061        if self.pa
-00029110: 6765 5f6e 756d 6265 7220 6973 206e 6f74  ge_number is not
-00029120: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00029130: 2020 2072 6573 756c 745b 2750 6167 654e     result['PageN
-00029140: 756d 6265 7227 5d20 3d20 7365 6c66 2e70  umber'] = self.p
-00029150: 6167 655f 6e75 6d62 6572 0a20 2020 2020  age_number.     
-00029160: 2020 2069 6620 7365 6c66 2e70 6167 655f     if self.page_
-00029170: 7369 7a65 2069 7320 6e6f 7420 4e6f 6e65  size is not None
-00029180: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00029190: 7375 6c74 5b27 5061 6765 5369 7a65 275d  sult['PageSize']
-000291a0: 203d 2073 656c 662e 7061 6765 5f73 697a   = self.page_siz
-000291b0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-000291c0: 662e 7069 7065 6c69 6e65 5f69 6420 6973  f.pipeline_id is
-000291d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000291e0: 2020 2020 2020 2072 6573 756c 745b 2750         result['P
-000291f0: 6970 656c 696e 6549 6427 5d20 3d20 7365  ipelineId'] = se
-00029200: 6c66 2e70 6970 656c 696e 655f 6964 0a20  lf.pipeline_id. 
-00029210: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-00029220: 6573 6f75 7263 655f 6964 2069 7320 6e6f  esource_id is no
-00029230: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00029240: 2020 2020 7265 7375 6c74 5b27 5265 736f      result['Reso
-00029250: 7572 6365 4964 275d 203d 2073 656c 662e  urceId'] = self.
-00029260: 7265 736f 7572 6365 5f69 640a 2020 2020  resource_id.    
-00029270: 2020 2020 6966 2073 656c 662e 7368 6f77      if self.show
-00029280: 5f6f 776e 2069 7320 6e6f 7420 4e6f 6e65  _own is not None
-00029290: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000292a0: 7375 6c74 5b27 5368 6f77 4f77 6e27 5d20  sult['ShowOwn'] 
-000292b0: 3d20 7365 6c66 2e73 686f 775f 6f77 6e0a  = self.show_own.
-000292c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000292d0: 736f 7274 5f62 7920 6973 206e 6f74 204e  sort_by is not N
-000292e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000292f0: 2072 6573 756c 745b 2753 6f72 7442 7927   result['SortBy'
-00029300: 5d20 3d20 7365 6c66 2e73 6f72 745f 6279  ] = self.sort_by
-00029310: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00029320: 2e73 7461 7274 5f74 696d 6520 6973 206e  .start_time is n
-00029330: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00029340: 2020 2020 2072 6573 756c 745b 2753 7461       result['Sta
-00029350: 7274 5469 6d65 275d 203d 2073 656c 662e  rtTime'] = self.
-00029360: 7374 6172 745f 7469 6d65 0a20 2020 2020  start_time.     
-00029370: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-00029380: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00029390: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000293a0: 745b 2753 7461 7475 7327 5d20 3d20 7365  t['Status'] = se
-000293b0: 6c66 2e73 7461 7475 730a 2020 2020 2020  lf.status.      
-000293c0: 2020 6966 2073 656c 662e 7461 6773 2069    if self.tags i
-000293d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000293e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000293f0: 5461 6773 275d 203d 2073 656c 662e 7461  Tags'] = self.ta
-00029400: 6773 0a20 2020 2020 2020 2069 6620 7365  gs.        if se
-00029410: 6c66 2e77 6f72 6b73 7061 6365 5f69 6420  lf.workspace_id 
-00029420: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00029430: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00029440: 2757 6f72 6b73 7061 6365 4964 275d 203d  'WorkspaceId'] =
-00029450: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
-00029460: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-00029470: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-00029480: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-00029490: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-000294a0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-000294b0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000294c0: 6574 2827 4275 7369 6e65 7373 5573 6572  et('BusinessUser
-000294d0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-000294e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000294f0: 6c66 2e62 7573 696e 6573 735f 7573 6572  lf.business_user
-00029500: 5f69 6420 3d20 6d2e 6765 7428 2742 7573  _id = m.get('Bus
-00029510: 696e 6573 7355 7365 7249 6427 290a 2020  inessUserId').  
-00029520: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00029530: 4361 6c6c 6572 2729 2069 7320 6e6f 7420  Caller') is not 
-00029540: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00029550: 2020 7365 6c66 2e63 616c 6c65 7220 3d20    self.caller = 
-00029560: 6d2e 6765 7428 2743 616c 6c65 7227 290a  m.get('Caller').
-00029570: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00029580: 2827 4469 7370 6c61 794e 616d 6527 2920  ('DisplayName') 
-00029590: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000295a0: 2020 2020 2020 2020 2073 656c 662e 6469           self.di
-000295b0: 7370 6c61 795f 6e61 6d65 203d 206d 2e67  splay_name = m.g
-000295c0: 6574 2827 4469 7370 6c61 794e 616d 6527  et('DisplayName'
-000295d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000295e0: 6574 2827 456e 6454 696d 6527 2920 6973  et('EndTime') is
-000295f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00029600: 2020 2020 2020 2073 656c 662e 656e 645f         self.end_
-00029610: 7469 6d65 203d 206d 2e67 6574 2827 456e  time = m.get('En
-00029620: 6454 696d 6527 290a 2020 2020 2020 2020  dTime').        
-00029630: 6966 206d 2e67 6574 2827 4672 6f6d 416c  if m.get('FromAl
-00029640: 6c57 6f72 6b73 7061 6365 7327 2920 6973  lWorkspaces') is
-00029650: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00029660: 2020 2020 2020 2073 656c 662e 6672 6f6d         self.from
-00029670: 5f61 6c6c 5f77 6f72 6b73 7061 6365 7320  _all_workspaces 
-00029680: 3d20 6d2e 6765 7428 2746 726f 6d41 6c6c  = m.get('FromAll
-00029690: 576f 726b 7370 6163 6573 2729 0a20 2020  Workspaces').   
-000296a0: 2020 2020 2069 6620 6d2e 6765 7428 274a       if m.get('J
-000296b0: 6f62 4964 2729 2069 7320 6e6f 7420 4e6f  obId') is not No
-000296c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000296d0: 7365 6c66 2e6a 6f62 5f69 6420 3d20 6d2e  self.job_id = m.
-000296e0: 6765 7428 274a 6f62 4964 2729 0a20 2020  get('JobId').   
-000296f0: 2020 2020 2069 6620 6d2e 6765 7428 274a       if m.get('J
-00029700: 6f62 5479 7065 2729 2069 7320 6e6f 7420  obType') is not 
-00029710: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00029720: 2020 7365 6c66 2e6a 6f62 5f74 7970 6520    self.job_type 
-00029730: 3d20 6d2e 6765 7428 274a 6f62 5479 7065  = m.get('JobType
-00029740: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00029750: 6765 7428 274f 7264 6572 2729 2069 7320  get('Order') is 
-00029760: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029770: 2020 2020 2020 7365 6c66 2e6f 7264 6572        self.order
-00029780: 203d 206d 2e67 6574 2827 4f72 6465 7227   = m.get('Order'
-00029790: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000297a0: 6574 2827 5061 6765 4e75 6d62 6572 2729  et('PageNumber')
-000297b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000297c0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000297d0: 6167 655f 6e75 6d62 6572 203d 206d 2e67  age_number = m.g
-000297e0: 6574 2827 5061 6765 4e75 6d62 6572 2729  et('PageNumber')
-000297f0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00029800: 7428 2750 6167 6553 697a 6527 2920 6973  t('PageSize') is
-00029810: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00029820: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
-00029830: 5f73 697a 6520 3d20 6d2e 6765 7428 2750  _size = m.get('P
-00029840: 6167 6553 697a 6527 290a 2020 2020 2020  ageSize').      
-00029850: 2020 6966 206d 2e67 6574 2827 5069 7065    if m.get('Pipe
-00029860: 6c69 6e65 4964 2729 2069 7320 6e6f 7420  lineId') is not 
-00029870: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00029880: 2020 7365 6c66 2e70 6970 656c 696e 655f    self.pipeline_
-00029890: 6964 203d 206d 2e67 6574 2827 5069 7065  id = m.get('Pipe
-000298a0: 6c69 6e65 4964 2729 0a20 2020 2020 2020  lineId').       
-000298b0: 2069 6620 6d2e 6765 7428 2752 6573 6f75   if m.get('Resou
-000298c0: 7263 6549 6427 2920 6973 206e 6f74 204e  rceId') is not N
-000298d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000298e0: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
-000298f0: 6420 3d20 6d2e 6765 7428 2752 6573 6f75  d = m.get('Resou
-00029900: 7263 6549 6427 290a 2020 2020 2020 2020  rceId').        
-00029910: 6966 206d 2e67 6574 2827 5368 6f77 4f77  if m.get('ShowOw
-00029920: 6e27 2920 6973 206e 6f74 204e 6f6e 653a  n') is not None:
-00029930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00029940: 662e 7368 6f77 5f6f 776e 203d 206d 2e67  f.show_own = m.g
-00029950: 6574 2827 5368 6f77 4f77 6e27 290a 2020  et('ShowOwn').  
-00029960: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00029970: 536f 7274 4279 2729 2069 7320 6e6f 7420  SortBy') is not 
-00029980: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00029990: 2020 7365 6c66 2e73 6f72 745f 6279 203d    self.sort_by =
-000299a0: 206d 2e67 6574 2827 536f 7274 4279 2729   m.get('SortBy')
-000299b0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000299c0: 7428 2753 7461 7274 5469 6d65 2729 2069  t('StartTime') i
-000299d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000299e0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-000299f0: 7274 5f74 696d 6520 3d20 6d2e 6765 7428  rt_time = m.get(
-00029a00: 2753 7461 7274 5469 6d65 2729 0a20 2020  'StartTime').   
-00029a10: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
-00029a20: 7461 7475 7327 2920 6973 206e 6f74 204e  tatus') is not N
-00029a30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00029a40: 2073 656c 662e 7374 6174 7573 203d 206d   self.status = m
-00029a50: 2e67 6574 2827 5374 6174 7573 2729 0a20  .get('Status'). 
-00029a60: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00029a70: 2754 6167 7327 2920 6973 206e 6f74 204e  'Tags') is not N
-00029a80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00029a90: 2073 656c 662e 7461 6773 203d 206d 2e67   self.tags = m.g
-00029aa0: 6574 2827 5461 6773 2729 0a20 2020 2020  et('Tags').     
-00029ab0: 2020 2069 6620 6d2e 6765 7428 2757 6f72     if m.get('Wor
-00029ac0: 6b73 7061 6365 4964 2729 2069 7320 6e6f  kspaceId') is no
-00029ad0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00029ae0: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
-00029af0: 6365 5f69 6420 3d20 6d2e 6765 7428 2757  ce_id = m.get('W
-00029b00: 6f72 6b73 7061 6365 4964 2729 0a20 2020  orkspaceId').   
-00029b10: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00029b20: 0a0a 0a63 6c61 7373 204c 6973 744a 6f62  ...class ListJob
-00029b30: 7353 6872 696e 6b52 6571 7565 7374 2854  sShrinkRequest(T
-00029b40: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-00029b50: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00029b60: 2062 7573 696e 6573 735f 7573 6572 5f69   business_user_i
-00029b70: 643d 4e6f 6e65 2c20 6361 6c6c 6572 3d4e  d=None, caller=N
-00029b80: 6f6e 652c 2064 6973 706c 6179 5f6e 616d  one, display_nam
-00029b90: 653d 4e6f 6e65 2c20 656e 645f 7469 6d65  e=None, end_time
-00029ba0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00029bb0: 2020 2020 2020 2020 6672 6f6d 5f61 6c6c          from_all
-00029bc0: 5f77 6f72 6b73 7061 6365 733d 4e6f 6e65  _workspaces=None
-00029bd0: 2c20 6a6f 625f 6964 3d4e 6f6e 652c 206a  , job_id=None, j
-00029be0: 6f62 5f74 7970 653d 4e6f 6e65 2c20 6f72  ob_type=None, or
-00029bf0: 6465 723d 4e6f 6e65 2c20 7061 6765 5f6e  der=None, page_n
-00029c00: 756d 6265 723d 4e6f 6e65 2c20 7061 6765  umber=None, page
-00029c10: 5f73 697a 653d 4e6f 6e65 2c20 7069 7065  _size=None, pipe
-00029c20: 6c69 6e65 5f69 643d 4e6f 6e65 2c0a 2020  line_id=None,.  
-00029c30: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00029c40: 6573 6f75 7263 655f 6964 3d4e 6f6e 652c  esource_id=None,
-00029c50: 2073 686f 775f 6f77 6e3d 4e6f 6e65 2c20   show_own=None, 
-00029c60: 736f 7274 5f62 793d 4e6f 6e65 2c20 7374  sort_by=None, st
-00029c70: 6172 745f 7469 6d65 3d4e 6f6e 652c 2073  art_time=None, s
-00029c80: 7461 7475 733d 4e6f 6e65 2c20 7461 6773  tatus=None, tags
-00029c90: 5f73 6872 696e 6b3d 4e6f 6e65 2c0a 2020  _shrink=None,.  
-00029ca0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00029cb0: 6f72 6b73 7061 6365 5f69 643d 4e6f 6e65  orkspace_id=None
-00029cc0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00029cd0: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
-00029ce0: 203d 2062 7573 696e 6573 735f 7573 6572   = business_user
-00029cf0: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
-00029d00: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
-00029d10: 6c6c 6572 203d 2063 616c 6c65 7220 2023  ller = caller  #
-00029d20: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-00029d30: 2020 2073 656c 662e 6469 7370 6c61 795f     self.display_
-00029d40: 6e61 6d65 203d 2064 6973 706c 6179 5f6e  name = display_n
-00029d50: 616d 6520 2023 2074 7970 653a 2073 7472  ame  # type: str
-00029d60: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-00029d70: 645f 7469 6d65 203d 2065 6e64 5f74 696d  d_time = end_tim
-00029d80: 6520 2023 2074 7970 653a 2073 7472 0a20  e  # type: str. 
-00029d90: 2020 2020 2020 2073 656c 662e 6672 6f6d         self.from
-00029da0: 5f61 6c6c 5f77 6f72 6b73 7061 6365 7320  _all_workspaces 
-00029db0: 3d20 6672 6f6d 5f61 6c6c 5f77 6f72 6b73  = from_all_works
-00029dc0: 7061 6365 7320 2023 2074 7970 653a 2062  paces  # type: b
-00029dd0: 6f6f 6c0a 2020 2020 2020 2020 7365 6c66  ool.        self
-00029de0: 2e6a 6f62 5f69 6420 3d20 6a6f 625f 6964  .job_id = job_id
-00029df0: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-00029e00: 2020 2020 2020 7365 6c66 2e6a 6f62 5f74        self.job_t
-00029e10: 7970 6520 3d20 6a6f 625f 7479 7065 2020  ype = job_type  
-00029e20: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00029e30: 2020 2020 7365 6c66 2e6f 7264 6572 203d      self.order =
-00029e40: 206f 7264 6572 2020 2320 7479 7065 3a20   order  # type: 
-00029e50: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-00029e60: 2e70 6167 655f 6e75 6d62 6572 203d 2070  .page_number = p
-00029e70: 6167 655f 6e75 6d62 6572 2020 2320 7479  age_number  # ty
-00029e80: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
-00029e90: 7365 6c66 2e70 6167 655f 7369 7a65 203d  self.page_size =
-00029ea0: 2070 6167 655f 7369 7a65 2020 2320 7479   page_size  # ty
-00029eb0: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
-00029ec0: 7365 6c66 2e70 6970 656c 696e 655f 6964  self.pipeline_id
-00029ed0: 203d 2070 6970 656c 696e 655f 6964 2020   = pipeline_id  
-00029ee0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00029ef0: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
-00029f00: 655f 6964 203d 2072 6573 6f75 7263 655f  e_id = resource_
-00029f10: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-00029f20: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
-00029f30: 775f 6f77 6e20 3d20 7368 6f77 5f6f 776e  w_own = show_own
-00029f40: 2020 2320 7479 7065 3a20 626f 6f6c 0a20    # type: bool. 
-00029f50: 2020 2020 2020 2073 656c 662e 736f 7274         self.sort
-00029f60: 5f62 7920 3d20 736f 7274 5f62 7920 2023  _by = sort_by  #
-00029f70: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-00029f80: 2020 2073 656c 662e 7374 6172 745f 7469     self.start_ti
-00029f90: 6d65 203d 2073 7461 7274 5f74 696d 6520  me = start_time 
-00029fa0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-00029fb0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00029fc0: 203d 2073 7461 7475 7320 2023 2074 7970   = status  # typ
-00029fd0: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-00029fe0: 656c 662e 7461 6773 5f73 6872 696e 6b20  elf.tags_shrink 
-00029ff0: 3d20 7461 6773 5f73 6872 696e 6b20 2023  = tags_shrink  #
-0002a000: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0002a010: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
-0002a020: 655f 6964 203d 2077 6f72 6b73 7061 6365  e_id = workspace
-0002a030: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
-0002a040: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0002a050: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0002a060: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-0002a070: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0002a080: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0002a090: 6572 284c 6973 744a 6f62 7353 6872 696e  er(ListJobsShrin
-0002a0a0: 6b52 6571 7565 7374 2c20 7365 6c66 292e  kRequest, self).
-0002a0b0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0002a0c0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-0002a0d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002a0e0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-0002a0f0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0002a100: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0002a110: 6620 7365 6c66 2e62 7573 696e 6573 735f  f self.business_
-0002a120: 7573 6572 5f69 6420 6973 206e 6f74 204e  user_id is not N
-0002a130: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002a140: 2072 6573 756c 745b 2742 7573 696e 6573   result['Busines
-0002a150: 7355 7365 7249 6427 5d20 3d20 7365 6c66  sUserId'] = self
-0002a160: 2e62 7573 696e 6573 735f 7573 6572 5f69  .business_user_i
-0002a170: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-0002a180: 662e 6361 6c6c 6572 2069 7320 6e6f 7420  f.caller is not 
-0002a190: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002a1a0: 2020 7265 7375 6c74 5b27 4361 6c6c 6572    result['Caller
-0002a1b0: 275d 203d 2073 656c 662e 6361 6c6c 6572  '] = self.caller
-0002a1c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002a1d0: 2e64 6973 706c 6179 5f6e 616d 6520 6973  .display_name is
-0002a1e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002a1f0: 2020 2020 2020 2072 6573 756c 745b 2744         result['D
-0002a200: 6973 706c 6179 4e61 6d65 275d 203d 2073  isplayName'] = s
-0002a210: 656c 662e 6469 7370 6c61 795f 6e61 6d65  elf.display_name
-0002a220: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002a230: 2e65 6e64 5f74 696d 6520 6973 206e 6f74  .end_time is not
-0002a240: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002a250: 2020 2072 6573 756c 745b 2745 6e64 5469     result['EndTi
-0002a260: 6d65 275d 203d 2073 656c 662e 656e 645f  me'] = self.end_
-0002a270: 7469 6d65 0a20 2020 2020 2020 2069 6620  time.        if 
-0002a280: 7365 6c66 2e66 726f 6d5f 616c 6c5f 776f  self.from_all_wo
-0002a290: 726b 7370 6163 6573 2069 7320 6e6f 7420  rkspaces is not 
-0002a2a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002a2b0: 2020 7265 7375 6c74 5b27 4672 6f6d 416c    result['FromAl
-0002a2c0: 6c57 6f72 6b73 7061 6365 7327 5d20 3d20  lWorkspaces'] = 
-0002a2d0: 7365 6c66 2e66 726f 6d5f 616c 6c5f 776f  self.from_all_wo
-0002a2e0: 726b 7370 6163 6573 0a20 2020 2020 2020  rkspaces.       
-0002a2f0: 2069 6620 7365 6c66 2e6a 6f62 5f69 6420   if self.job_id 
-0002a300: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002a310: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002a320: 274a 6f62 4964 275d 203d 2073 656c 662e  'JobId'] = self.
-0002a330: 6a6f 625f 6964 0a20 2020 2020 2020 2069  job_id.        i
-0002a340: 6620 7365 6c66 2e6a 6f62 5f74 7970 6520  f self.job_type 
-0002a350: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002a360: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002a370: 274a 6f62 5479 7065 275d 203d 2073 656c  'JobType'] = sel
-0002a380: 662e 6a6f 625f 7479 7065 0a20 2020 2020  f.job_type.     
-0002a390: 2020 2069 6620 7365 6c66 2e6f 7264 6572     if self.order
-0002a3a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002a3b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002a3c0: 5b27 4f72 6465 7227 5d20 3d20 7365 6c66  ['Order'] = self
-0002a3d0: 2e6f 7264 6572 0a20 2020 2020 2020 2069  .order.        i
-0002a3e0: 6620 7365 6c66 2e70 6167 655f 6e75 6d62  f self.page_numb
-0002a3f0: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-0002a400: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002a410: 6c74 5b27 5061 6765 4e75 6d62 6572 275d  lt['PageNumber']
-0002a420: 203d 2073 656c 662e 7061 6765 5f6e 756d   = self.page_num
-0002a430: 6265 720a 2020 2020 2020 2020 6966 2073  ber.        if s
-0002a440: 656c 662e 7061 6765 5f73 697a 6520 6973  elf.page_size is
-0002a450: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002a460: 2020 2020 2020 2072 6573 756c 745b 2750         result['P
-0002a470: 6167 6553 697a 6527 5d20 3d20 7365 6c66  ageSize'] = self
-0002a480: 2e70 6167 655f 7369 7a65 0a20 2020 2020  .page_size.     
-0002a490: 2020 2069 6620 7365 6c66 2e70 6970 656c     if self.pipel
-0002a4a0: 696e 655f 6964 2069 7320 6e6f 7420 4e6f  ine_id is not No
-0002a4b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002a4c0: 7265 7375 6c74 5b27 5069 7065 6c69 6e65  result['Pipeline
-0002a4d0: 4964 275d 203d 2073 656c 662e 7069 7065  Id'] = self.pipe
-0002a4e0: 6c69 6e65 5f69 640a 2020 2020 2020 2020  line_id.        
-0002a4f0: 6966 2073 656c 662e 7265 736f 7572 6365  if self.resource
-0002a500: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-0002a510: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002a520: 756c 745b 2752 6573 6f75 7263 6549 6427  ult['ResourceId'
-0002a530: 5d20 3d20 7365 6c66 2e72 6573 6f75 7263  ] = self.resourc
-0002a540: 655f 6964 0a20 2020 2020 2020 2069 6620  e_id.        if 
-0002a550: 7365 6c66 2e73 686f 775f 6f77 6e20 6973  self.show_own is
-0002a560: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002a570: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
-0002a580: 686f 774f 776e 275d 203d 2073 656c 662e  howOwn'] = self.
-0002a590: 7368 6f77 5f6f 776e 0a20 2020 2020 2020  show_own.       
-0002a5a0: 2069 6620 7365 6c66 2e73 6f72 745f 6279   if self.sort_by
-0002a5b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002a5c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002a5d0: 5b27 536f 7274 4279 275d 203d 2073 656c  ['SortBy'] = sel
-0002a5e0: 662e 736f 7274 5f62 790a 2020 2020 2020  f.sort_by.      
-0002a5f0: 2020 6966 2073 656c 662e 7374 6172 745f    if self.start_
-0002a600: 7469 6d65 2069 7320 6e6f 7420 4e6f 6e65  time is not None
-0002a610: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002a620: 7375 6c74 5b27 5374 6172 7454 696d 6527  sult['StartTime'
-0002a630: 5d20 3d20 7365 6c66 2e73 7461 7274 5f74  ] = self.start_t
-0002a640: 696d 650a 2020 2020 2020 2020 6966 2073  ime.        if s
-0002a650: 656c 662e 7374 6174 7573 2069 7320 6e6f  elf.status is no
-0002a660: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002a670: 2020 2020 7265 7375 6c74 5b27 5374 6174      result['Stat
-0002a680: 7573 275d 203d 2073 656c 662e 7374 6174  us'] = self.stat
-0002a690: 7573 0a20 2020 2020 2020 2069 6620 7365  us.        if se
-0002a6a0: 6c66 2e74 6167 735f 7368 7269 6e6b 2069  lf.tags_shrink i
-0002a6b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002a6c0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002a6d0: 5461 6773 275d 203d 2073 656c 662e 7461  Tags'] = self.ta
-0002a6e0: 6773 5f73 6872 696e 6b0a 2020 2020 2020  gs_shrink.      
-0002a6f0: 2020 6966 2073 656c 662e 776f 726b 7370    if self.worksp
-0002a700: 6163 655f 6964 2069 7320 6e6f 7420 4e6f  ace_id is not No
-0002a710: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002a720: 7265 7375 6c74 5b27 576f 726b 7370 6163  result['Workspac
-0002a730: 6549 6427 5d20 3d20 7365 6c66 2e77 6f72  eId'] = self.wor
-0002a740: 6b73 7061 6365 5f69 640a 2020 2020 2020  kspace_id.      
-0002a750: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0002a760: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0002a770: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-0002a780: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-0002a790: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-0002a7a0: 2069 6620 6d2e 6765 7428 2742 7573 696e   if m.get('Busin
-0002a7b0: 6573 7355 7365 7249 6427 2920 6973 206e  essUserId') is n
-0002a7c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002a7d0: 2020 2020 2073 656c 662e 6275 7369 6e65       self.busine
-0002a7e0: 7373 5f75 7365 725f 6964 203d 206d 2e67  ss_user_id = m.g
-0002a7f0: 6574 2827 4275 7369 6e65 7373 5573 6572  et('BusinessUser
-0002a800: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-0002a810: 6d2e 6765 7428 2743 616c 6c65 7227 2920  m.get('Caller') 
-0002a820: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002a830: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
-0002a840: 6c6c 6572 203d 206d 2e67 6574 2827 4361  ller = m.get('Ca
-0002a850: 6c6c 6572 2729 0a20 2020 2020 2020 2069  ller').        i
-0002a860: 6620 6d2e 6765 7428 2744 6973 706c 6179  f m.get('Display
-0002a870: 4e61 6d65 2729 2069 7320 6e6f 7420 4e6f  Name') is not No
-0002a880: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002a890: 7365 6c66 2e64 6973 706c 6179 5f6e 616d  self.display_nam
-0002a8a0: 6520 3d20 6d2e 6765 7428 2744 6973 706c  e = m.get('Displ
-0002a8b0: 6179 4e61 6d65 2729 0a20 2020 2020 2020  ayName').       
-0002a8c0: 2069 6620 6d2e 6765 7428 2745 6e64 5469   if m.get('EndTi
-0002a8d0: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
-0002a8e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002a8f0: 6c66 2e65 6e64 5f74 696d 6520 3d20 6d2e  lf.end_time = m.
-0002a900: 6765 7428 2745 6e64 5469 6d65 2729 0a20  get('EndTime'). 
-0002a910: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002a920: 2746 726f 6d41 6c6c 576f 726b 7370 6163  'FromAllWorkspac
-0002a930: 6573 2729 2069 7320 6e6f 7420 4e6f 6e65  es') is not None
-0002a940: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002a950: 6c66 2e66 726f 6d5f 616c 6c5f 776f 726b  lf.from_all_work
-0002a960: 7370 6163 6573 203d 206d 2e67 6574 2827  spaces = m.get('
-0002a970: 4672 6f6d 416c 6c57 6f72 6b73 7061 6365  FromAllWorkspace
-0002a980: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-0002a990: 2e67 6574 2827 4a6f 6249 6427 2920 6973  .get('JobId') is
-0002a9a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002a9b0: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
-0002a9c0: 6964 203d 206d 2e67 6574 2827 4a6f 6249  id = m.get('JobI
-0002a9d0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-0002a9e0: 2e67 6574 2827 4a6f 6254 7970 6527 2920  .get('JobType') 
-0002a9f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002aa00: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
-0002aa10: 625f 7479 7065 203d 206d 2e67 6574 2827  b_type = m.get('
-0002aa20: 4a6f 6254 7970 6527 290a 2020 2020 2020  JobType').      
-0002aa30: 2020 6966 206d 2e67 6574 2827 4f72 6465    if m.get('Orde
-0002aa40: 7227 2920 6973 206e 6f74 204e 6f6e 653a  r') is not None:
-0002aa50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002aa60: 662e 6f72 6465 7220 3d20 6d2e 6765 7428  f.order = m.get(
-0002aa70: 274f 7264 6572 2729 0a20 2020 2020 2020  'Order').       
-0002aa80: 2069 6620 6d2e 6765 7428 2750 6167 654e   if m.get('PageN
-0002aa90: 756d 6265 7227 2920 6973 206e 6f74 204e  umber') is not N
-0002aaa0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002aab0: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
-0002aac0: 7220 3d20 6d2e 6765 7428 2750 6167 654e  r = m.get('PageN
-0002aad0: 756d 6265 7227 290a 2020 2020 2020 2020  umber').        
-0002aae0: 6966 206d 2e67 6574 2827 5061 6765 5369  if m.get('PageSi
-0002aaf0: 7a65 2729 2069 7320 6e6f 7420 4e6f 6e65  ze') is not None
-0002ab00: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002ab10: 6c66 2e70 6167 655f 7369 7a65 203d 206d  lf.page_size = m
-0002ab20: 2e67 6574 2827 5061 6765 5369 7a65 2729  .get('PageSize')
-0002ab30: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002ab40: 7428 2750 6970 656c 696e 6549 6427 2920  t('PipelineId') 
-0002ab50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002ab60: 2020 2020 2020 2020 2073 656c 662e 7069           self.pi
-0002ab70: 7065 6c69 6e65 5f69 6420 3d20 6d2e 6765  peline_id = m.ge
-0002ab80: 7428 2750 6970 656c 696e 6549 6427 290a  t('PipelineId').
-0002ab90: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002aba0: 2827 5265 736f 7572 6365 4964 2729 2069  ('ResourceId') i
-0002abb0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002abc0: 2020 2020 2020 2020 7365 6c66 2e72 6573          self.res
-0002abd0: 6f75 7263 655f 6964 203d 206d 2e67 6574  ource_id = m.get
-0002abe0: 2827 5265 736f 7572 6365 4964 2729 0a20  ('ResourceId'). 
-0002abf0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002ac00: 2753 686f 774f 776e 2729 2069 7320 6e6f  'ShowOwn') is no
-0002ac10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002ac20: 2020 2020 7365 6c66 2e73 686f 775f 6f77      self.show_ow
-0002ac30: 6e20 3d20 6d2e 6765 7428 2753 686f 774f  n = m.get('ShowO
-0002ac40: 776e 2729 0a20 2020 2020 2020 2069 6620  wn').        if 
-0002ac50: 6d2e 6765 7428 2753 6f72 7442 7927 2920  m.get('SortBy') 
-0002ac60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002ac70: 2020 2020 2020 2020 2073 656c 662e 736f           self.so
-0002ac80: 7274 5f62 7920 3d20 6d2e 6765 7428 2753  rt_by = m.get('S
-0002ac90: 6f72 7442 7927 290a 2020 2020 2020 2020  ortBy').        
-0002aca0: 6966 206d 2e67 6574 2827 5374 6172 7454  if m.get('StartT
-0002acb0: 696d 6527 2920 6973 206e 6f74 204e 6f6e  ime') is not Non
-0002acc0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002acd0: 656c 662e 7374 6172 745f 7469 6d65 203d  elf.start_time =
-0002ace0: 206d 2e67 6574 2827 5374 6172 7454 696d   m.get('StartTim
-0002acf0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-0002ad00: 2e67 6574 2827 5374 6174 7573 2729 2069  .get('Status') i
-0002ad10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002ad20: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0002ad30: 7475 7320 3d20 6d2e 6765 7428 2753 7461  tus = m.get('Sta
-0002ad40: 7475 7327 290a 2020 2020 2020 2020 6966  tus').        if
-0002ad50: 206d 2e67 6574 2827 5461 6773 2729 2069   m.get('Tags') i
-0002ad60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002ad70: 2020 2020 2020 2020 7365 6c66 2e74 6167          self.tag
-0002ad80: 735f 7368 7269 6e6b 203d 206d 2e67 6574  s_shrink = m.get
-0002ad90: 2827 5461 6773 2729 0a20 2020 2020 2020  ('Tags').       
-0002ada0: 2069 6620 6d2e 6765 7428 2757 6f72 6b73   if m.get('Works
-0002adb0: 7061 6365 4964 2729 2069 7320 6e6f 7420  paceId') is not 
-0002adc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002add0: 2020 7365 6c66 2e77 6f72 6b73 7061 6365    self.workspace
-0002ade0: 5f69 6420 3d20 6d2e 6765 7428 2757 6f72  _id = m.get('Wor
-0002adf0: 6b73 7061 6365 4964 2729 0a20 2020 2020  kspaceId').     
-0002ae00: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0002ae10: 0a63 6c61 7373 204c 6973 744a 6f62 7352  .class ListJobsR
-0002ae20: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-0002ae30: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002ae40: 5f69 6e69 745f 5f28 7365 6c66 2c20 6a6f  _init__(self, jo
-0002ae50: 6273 3d4e 6f6e 652c 2072 6571 7565 7374  bs=None, request
-0002ae60: 5f69 643d 4e6f 6e65 2c20 746f 7461 6c5f  _id=None, total_
-0002ae70: 636f 756e 743d 4e6f 6e65 293a 0a20 2020  count=None):.   
-0002ae80: 2020 2020 2073 656c 662e 6a6f 6273 203d       self.jobs =
-0002ae90: 206a 6f62 7320 2023 2074 7970 653a 206c   jobs  # type: l
-0002aea0: 6973 745b 4a6f 6249 7465 6d5d 0a20 2020  ist[JobItem].   
-0002aeb0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-0002aec0: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
-0002aed0: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
-0002aee0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
-0002aef0: 6c5f 636f 756e 7420 3d20 746f 7461 6c5f  l_count = total_
-0002af00: 636f 756e 7420 2023 2074 7970 653a 206c  count  # type: l
-0002af10: 6f6e 670a 0a20 2020 2064 6566 2076 616c  ong..    def val
-0002af20: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0002af30: 2020 2020 2069 6620 7365 6c66 2e6a 6f62       if self.job
-0002af40: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-0002af50: 6f72 206b 2069 6e20 7365 6c66 2e6a 6f62  or k in self.job
-0002af60: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0002af70: 2020 2069 6620 6b3a 0a20 2020 2020 2020     if k:.       
-0002af80: 2020 2020 2020 2020 2020 2020 206b 2e76               k.v
-0002af90: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
-0002afa0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-0002afb0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-0002afc0: 7375 7065 7228 4c69 7374 4a6f 6273 5265  super(ListJobsRe
-0002afd0: 7370 6f6e 7365 426f 6479 2c20 7365 6c66  sponseBody, self
-0002afe0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0002aff0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0002b000: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002b010: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0002b020: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0002b030: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0002b040: 2072 6573 756c 745b 274a 6f62 7327 5d20   result['Jobs'] 
-0002b050: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
-0002b060: 7365 6c66 2e6a 6f62 7320 6973 206e 6f74  self.jobs is not
-0002b070: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002b080: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
-0002b090: 2e6a 6f62 733a 0a20 2020 2020 2020 2020  .jobs:.         
-0002b0a0: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
-0002b0b0: 6f62 7327 5d2e 6170 7065 6e64 286b 2e74  obs'].append(k.t
-0002b0c0: 6f5f 6d61 7028 2920 6966 206b 2065 6c73  o_map() if k els
-0002b0d0: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
-0002b0e0: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
-0002b0f0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0002b100: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002b110: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
-0002b120: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
-0002b130: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-0002b140: 662e 746f 7461 6c5f 636f 756e 7420 6973  f.total_count is
-0002b150: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002b160: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
-0002b170: 6f74 616c 436f 756e 7427 5d20 3d20 7365  otalCount'] = se
-0002b180: 6c66 2e74 6f74 616c 5f63 6f75 6e74 0a20  lf.total_count. 
-0002b190: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002b1a0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0002b1b0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-0002b1c0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0002b1d0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0002b1e0: 2020 2020 2020 7365 6c66 2e6a 6f62 7320        self.jobs 
-0002b1f0: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
-0002b200: 6d2e 6765 7428 274a 6f62 7327 2920 6973  m.get('Jobs') is
-0002b210: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002b220: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-0002b230: 6d2e 6765 7428 274a 6f62 7327 293a 0a20  m.get('Jobs'):. 
-0002b240: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0002b250: 656d 705f 6d6f 6465 6c20 3d20 4a6f 6249  emp_model = JobI
-0002b260: 7465 6d28 290a 2020 2020 2020 2020 2020  tem().          
-0002b270: 2020 2020 2020 7365 6c66 2e6a 6f62 732e        self.jobs.
-0002b280: 6170 7065 6e64 2874 656d 705f 6d6f 6465  append(temp_mode
-0002b290: 6c2e 6672 6f6d 5f6d 6170 286b 2929 0a20  l.from_map(k)). 
-0002b2a0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002b2b0: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
-0002b2c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002b2d0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-0002b2e0: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
-0002b2f0: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
-0002b300: 2020 2069 6620 6d2e 6765 7428 2754 6f74     if m.get('Tot
-0002b310: 616c 436f 756e 7427 2920 6973 206e 6f74  alCount') is not
-0002b320: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002b330: 2020 2073 656c 662e 746f 7461 6c5f 636f     self.total_co
-0002b340: 756e 7420 3d20 6d2e 6765 7428 2754 6f74  unt = m.get('Tot
-0002b350: 616c 436f 756e 7427 290a 2020 2020 2020  alCount').      
-0002b360: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0002b370: 636c 6173 7320 4c69 7374 4a6f 6273 5265  class ListJobsRe
-0002b380: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-0002b390: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0002b3a0: 5f5f 2873 656c 662c 2068 6561 6465 7273  __(self, headers
-0002b3b0: 3d4e 6f6e 652c 2073 7461 7475 735f 636f  =None, status_co
-0002b3c0: 6465 3d4e 6f6e 652c 2062 6f64 793d 4e6f  de=None, body=No
-0002b3d0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
-0002b3e0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-0002b3f0: 6572 7320 2023 2074 7970 653a 2064 6963  ers  # type: dic
-0002b400: 745b 7374 722c 2073 7472 5d0a 2020 2020  t[str, str].    
-0002b410: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-0002b420: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
-0002b430: 6465 2020 2320 7479 7065 3a20 696e 740a  de  # type: int.
-0002b440: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0002b450: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
-0002b460: 3a20 4c69 7374 4a6f 6273 5265 7370 6f6e  : ListJobsRespon
-0002b470: 7365 426f 6479 0a0a 2020 2020 6465 6620  seBody..    def 
-0002b480: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0002b490: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-0002b4a0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-0002b4b0: 656c 662e 6865 6164 6572 732c 2027 6865  elf.headers, 'he
-0002b4c0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-0002b4d0: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-0002b4e0: 7175 6972 6564 2873 656c 662e 7374 6174  quired(self.stat
-0002b4f0: 7573 5f63 6f64 652c 2027 7374 6174 7573  us_code, 'status
-0002b500: 5f63 6f64 6527 290a 2020 2020 2020 2020  _code').        
-0002b510: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-0002b520: 7175 6972 6564 2873 656c 662e 626f 6479  quired(self.body
-0002b530: 2c20 2762 6f64 7927 290a 2020 2020 2020  , 'body').      
-0002b540: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
-0002b550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002b560: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
-0002b570: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-0002b580: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002b590: 5f6d 6170 203d 2073 7570 6572 284c 6973  _map = super(Lis
-0002b5a0: 744a 6f62 7352 6573 706f 6e73 652c 2073  tJobsResponse, s
-0002b5b0: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
-0002b5c0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0002b5d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002b5e0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0002b5f0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0002b600: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0002b610: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
-0002b620: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-0002b630: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002b640: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
-0002b650: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
-0002b660: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-0002b670: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
-0002b680: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002b690: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
-0002b6a0: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
-0002b6b0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-0002b6c0: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-0002b6d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002b6e0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002b6f0: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-0002b700: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-0002b710: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0002b720: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0002b730: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
-0002b740: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0002b750: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0002b760: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
-0002b770: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
-0002b780: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002b790: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-0002b7a0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-0002b7b0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002b7c0: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
-0002b7d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002b7e0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-0002b7f0: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
-0002b800: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
-0002b810: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002b820: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
-0002b830: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002b840: 2020 7465 6d70 5f6d 6f64 656c 203d 204c    temp_model = L
-0002b850: 6973 744a 6f62 7352 6573 706f 6e73 6542  istJobsResponseB
-0002b860: 6f64 7928 290a 2020 2020 2020 2020 2020  ody().          
-0002b870: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
-0002b880: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-0002b890: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
-0002b8a0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0002b8b0: 0a0a 0a63 6c61 7373 204c 6973 7454 656e  ...class ListTen
-0002b8c0: 736f 7262 6f61 7264 7352 6571 7565 7374  sorboardsRequest
-0002b8d0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-0002b8e0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0002b8f0: 662c 2064 6973 706c 6179 5f6e 616d 653d  f, display_name=
-0002b900: 4e6f 6e65 2c20 656e 645f 7469 6d65 3d4e  None, end_time=N
-0002b910: 6f6e 652c 206a 6f62 5f69 643d 4e6f 6e65  one, job_id=None
-0002b920: 2c20 6f72 6465 723d 4e6f 6e65 2c20 7061  , order=None, pa
-0002b930: 6765 5f6e 756d 6265 723d 4e6f 6e65 2c20  ge_number=None, 
-0002b940: 7061 6765 5f73 697a 653d 4e6f 6e65 2c0a  page_size=None,.
-0002b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b960: 2073 6f72 745f 6279 3d4e 6f6e 652c 2073   sort_by=None, s
-0002b970: 6f75 7263 655f 6964 3d4e 6f6e 652c 2073  ource_id=None, s
-0002b980: 6f75 7263 655f 7479 7065 3d4e 6f6e 652c  ource_type=None,
-0002b990: 2073 7461 7274 5f74 696d 653d 4e6f 6e65   start_time=None
-0002b9a0: 2c20 7374 6174 7573 3d4e 6f6e 652c 2074  , status=None, t
-0002b9b0: 656e 736f 7262 6f61 7264 5f69 643d 4e6f  ensorboard_id=No
-0002b9c0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0002b9d0: 2020 2020 2076 6572 626f 7365 3d4e 6f6e       verbose=Non
-0002b9e0: 652c 2077 6f72 6b73 7061 6365 5f69 643d  e, workspace_id=
-0002b9f0: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-0002ba00: 656c 662e 6469 7370 6c61 795f 6e61 6d65  elf.display_name
-0002ba10: 203d 2064 6973 706c 6179 5f6e 616d 6520   = display_name 
-0002ba20: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-0002ba30: 2020 2020 2073 656c 662e 656e 645f 7469       self.end_ti
-0002ba40: 6d65 203d 2065 6e64 5f74 696d 6520 2023  me = end_time  #
-0002ba50: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0002ba60: 2020 2073 656c 662e 6a6f 625f 6964 203d     self.job_id =
-0002ba70: 206a 6f62 5f69 6420 2023 2074 7970 653a   job_id  # type:
-0002ba80: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
-0002ba90: 662e 6f72 6465 7220 3d20 6f72 6465 7220  f.order = order 
-0002baa0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-0002bab0: 2020 2020 2073 656c 662e 7061 6765 5f6e       self.page_n
-0002bac0: 756d 6265 7220 3d20 7061 6765 5f6e 756d  umber = page_num
-0002bad0: 6265 7220 2023 2074 7970 653a 2069 6e74  ber  # type: int
-0002bae0: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
-0002baf0: 6765 5f73 697a 6520 3d20 7061 6765 5f73  ge_size = page_s
-0002bb00: 697a 6520 2023 2074 7970 653a 2069 6e74  ize  # type: int
-0002bb10: 0a20 2020 2020 2020 2073 656c 662e 736f  .        self.so
-0002bb20: 7274 5f62 7920 3d20 736f 7274 5f62 7920  rt_by = sort_by 
-0002bb30: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-0002bb40: 2020 2020 2073 656c 662e 736f 7572 6365       self.source
-0002bb50: 5f69 6420 3d20 736f 7572 6365 5f69 6420  _id = source_id 
-0002bb60: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-0002bb70: 2020 2020 2073 656c 662e 736f 7572 6365       self.source
-0002bb80: 5f74 7970 6520 3d20 736f 7572 6365 5f74  _type = source_t
-0002bb90: 7970 6520 2023 2074 7970 653a 2073 7472  ype  # type: str
-0002bba0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0002bbb0: 6172 745f 7469 6d65 203d 2073 7461 7274  art_time = start
-0002bbc0: 5f74 696d 6520 2023 2074 7970 653a 2073  _time  # type: s
-0002bbd0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-0002bbe0: 7374 6174 7573 203d 2073 7461 7475 7320  status = status 
-0002bbf0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-0002bc00: 2020 2020 2073 656c 662e 7465 6e73 6f72       self.tensor
-0002bc10: 626f 6172 645f 6964 203d 2074 656e 736f  board_id = tenso
-0002bc20: 7262 6f61 7264 5f69 6420 2023 2074 7970  rboard_id  # typ
-0002bc30: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-0002bc40: 656c 662e 7665 7262 6f73 6520 3d20 7665  elf.verbose = ve
-0002bc50: 7262 6f73 6520 2023 2074 7970 653a 2062  rbose  # type: b
-0002bc60: 6f6f 6c0a 2020 2020 2020 2020 7365 6c66  ool.        self
-0002bc70: 2e77 6f72 6b73 7061 6365 5f69 6420 3d20  .workspace_id = 
-0002bc80: 776f 726b 7370 6163 655f 6964 2020 2320  workspace_id  # 
-0002bc90: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
-0002bca0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0002bcb0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0002bcc0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0002bcd0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0002bce0: 6d61 7020 3d20 7375 7065 7228 4c69 7374  map = super(List
-0002bcf0: 5465 6e73 6f72 626f 6172 6473 5265 7175  TensorboardsRequ
-0002bd00: 6573 742c 2073 656c 6629 2e74 6f5f 6d61  est, self).to_ma
-0002bd10: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0002bd20: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0002bd30: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0002bd40: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0002bd50: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0002bd60: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0002bd70: 662e 6469 7370 6c61 795f 6e61 6d65 2069  f.display_name i
-0002bd80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002bd90: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002bda0: 4469 7370 6c61 794e 616d 6527 5d20 3d20  DisplayName'] = 
-0002bdb0: 7365 6c66 2e64 6973 706c 6179 5f6e 616d  self.display_nam
-0002bdc0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0002bdd0: 662e 656e 645f 7469 6d65 2069 7320 6e6f  f.end_time is no
-0002bde0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002bdf0: 2020 2020 7265 7375 6c74 5b27 456e 6454      result['EndT
-0002be00: 696d 6527 5d20 3d20 7365 6c66 2e65 6e64  ime'] = self.end
-0002be10: 5f74 696d 650a 2020 2020 2020 2020 6966  _time.        if
-0002be20: 2073 656c 662e 6a6f 625f 6964 2069 7320   self.job_id is 
-0002be30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002be40: 2020 2020 2020 7265 7375 6c74 5b27 4a6f        result['Jo
-0002be50: 6249 6427 5d20 3d20 7365 6c66 2e6a 6f62  bId'] = self.job
-0002be60: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-0002be70: 656c 662e 6f72 6465 7220 6973 206e 6f74  elf.order is not
-0002be80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002be90: 2020 2072 6573 756c 745b 274f 7264 6572     result['Order
-0002bea0: 275d 203d 2073 656c 662e 6f72 6465 720a  '] = self.order.
-0002beb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002bec0: 7061 6765 5f6e 756d 6265 7220 6973 206e  page_number is n
-0002bed0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002bee0: 2020 2020 2072 6573 756c 745b 2750 6167       result['Pag
-0002bef0: 654e 756d 6265 7227 5d20 3d20 7365 6c66  eNumber'] = self
-0002bf00: 2e70 6167 655f 6e75 6d62 6572 0a20 2020  .page_number.   
-0002bf10: 2020 2020 2069 6620 7365 6c66 2e70 6167       if self.pag
-0002bf20: 655f 7369 7a65 2069 7320 6e6f 7420 4e6f  e_size is not No
-0002bf30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002bf40: 7265 7375 6c74 5b27 5061 6765 5369 7a65  result['PageSize
-0002bf50: 275d 203d 2073 656c 662e 7061 6765 5f73  '] = self.page_s
-0002bf60: 697a 650a 2020 2020 2020 2020 6966 2073  ize.        if s
-0002bf70: 656c 662e 736f 7274 5f62 7920 6973 206e  elf.sort_by is n
-0002bf80: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002bf90: 2020 2020 2072 6573 756c 745b 2753 6f72       result['Sor
-0002bfa0: 7442 7927 5d20 3d20 7365 6c66 2e73 6f72  tBy'] = self.sor
-0002bfb0: 745f 6279 0a20 2020 2020 2020 2069 6620  t_by.        if 
-0002bfc0: 7365 6c66 2e73 6f75 7263 655f 6964 2069  self.source_id i
-0002bfd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002bfe0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002bff0: 536f 7572 6365 4964 275d 203d 2073 656c  SourceId'] = sel
-0002c000: 662e 736f 7572 6365 5f69 640a 2020 2020  f.source_id.    
-0002c010: 2020 2020 6966 2073 656c 662e 736f 7572      if self.sour
-0002c020: 6365 5f74 7970 6520 6973 206e 6f74 204e  ce_type is not N
-0002c030: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002c040: 2072 6573 756c 745b 2753 6f75 7263 6554   result['SourceT
-0002c050: 7970 6527 5d20 3d20 7365 6c66 2e73 6f75  ype'] = self.sou
-0002c060: 7263 655f 7479 7065 0a20 2020 2020 2020  rce_type.       
-0002c070: 2069 6620 7365 6c66 2e73 7461 7274 5f74   if self.start_t
-0002c080: 696d 6520 6973 206e 6f74 204e 6f6e 653a  ime is not None:
-0002c090: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002c0a0: 756c 745b 2753 7461 7274 5469 6d65 275d  ult['StartTime']
-0002c0b0: 203d 2073 656c 662e 7374 6172 745f 7469   = self.start_ti
-0002c0c0: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
-0002c0d0: 6c66 2e73 7461 7475 7320 6973 206e 6f74  lf.status is not
-0002c0e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002c0f0: 2020 2072 6573 756c 745b 2753 7461 7475     result['Statu
-0002c100: 7327 5d20 3d20 7365 6c66 2e73 7461 7475  s'] = self.statu
-0002c110: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-0002c120: 662e 7465 6e73 6f72 626f 6172 645f 6964  f.tensorboard_id
-0002c130: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002c140: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002c150: 5b27 5465 6e73 6f72 626f 6172 6449 6427  ['TensorboardId'
-0002c160: 5d20 3d20 7365 6c66 2e74 656e 736f 7262  ] = self.tensorb
-0002c170: 6f61 7264 5f69 640a 2020 2020 2020 2020  oard_id.        
-0002c180: 6966 2073 656c 662e 7665 7262 6f73 6520  if self.verbose 
-0002c190: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002c1a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002c1b0: 2756 6572 626f 7365 275d 203d 2073 656c  'Verbose'] = sel
-0002c1c0: 662e 7665 7262 6f73 650a 2020 2020 2020  f.verbose.      
-0002c1d0: 2020 6966 2073 656c 662e 776f 726b 7370    if self.worksp
-0002c1e0: 6163 655f 6964 2069 7320 6e6f 7420 4e6f  ace_id is not No
-0002c1f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002c200: 7265 7375 6c74 5b27 576f 726b 7370 6163  result['Workspac
-0002c210: 6549 6427 5d20 3d20 7365 6c66 2e77 6f72  eId'] = self.wor
-0002c220: 6b73 7061 6365 5f69 640a 2020 2020 2020  kspace_id.      
-0002c230: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0002c240: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0002c250: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-0002c260: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-0002c270: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-0002c280: 2069 6620 6d2e 6765 7428 2744 6973 706c   if m.get('Displ
-0002c290: 6179 4e61 6d65 2729 2069 7320 6e6f 7420  ayName') is not 
-0002c2a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002c2b0: 2020 7365 6c66 2e64 6973 706c 6179 5f6e    self.display_n
-0002c2c0: 616d 6520 3d20 6d2e 6765 7428 2744 6973  ame = m.get('Dis
-0002c2d0: 706c 6179 4e61 6d65 2729 0a20 2020 2020  playName').     
-0002c2e0: 2020 2069 6620 6d2e 6765 7428 2745 6e64     if m.get('End
-0002c2f0: 5469 6d65 2729 2069 7320 6e6f 7420 4e6f  Time') is not No
-0002c300: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002c310: 7365 6c66 2e65 6e64 5f74 696d 6520 3d20  self.end_time = 
-0002c320: 6d2e 6765 7428 2745 6e64 5469 6d65 2729  m.get('EndTime')
-0002c330: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002c340: 7428 274a 6f62 4964 2729 2069 7320 6e6f  t('JobId') is no
-0002c350: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002c360: 2020 2020 7365 6c66 2e6a 6f62 5f69 6420      self.job_id 
-0002c370: 3d20 6d2e 6765 7428 274a 6f62 4964 2729  = m.get('JobId')
-0002c380: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002c390: 7428 274f 7264 6572 2729 2069 7320 6e6f  t('Order') is no
-0002c3a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002c3b0: 2020 2020 7365 6c66 2e6f 7264 6572 203d      self.order =
-0002c3c0: 206d 2e67 6574 2827 4f72 6465 7227 290a   m.get('Order').
-0002c3d0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002c3e0: 2827 5061 6765 4e75 6d62 6572 2729 2069  ('PageNumber') i
-0002c3f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002c400: 2020 2020 2020 2020 7365 6c66 2e70 6167          self.pag
-0002c410: 655f 6e75 6d62 6572 203d 206d 2e67 6574  e_number = m.get
-0002c420: 2827 5061 6765 4e75 6d62 6572 2729 0a20  ('PageNumber'). 
-0002c430: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002c440: 2750 6167 6553 697a 6527 2920 6973 206e  'PageSize') is n
-0002c450: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002c460: 2020 2020 2073 656c 662e 7061 6765 5f73       self.page_s
-0002c470: 697a 6520 3d20 6d2e 6765 7428 2750 6167  ize = m.get('Pag
-0002c480: 6553 697a 6527 290a 2020 2020 2020 2020  eSize').        
-0002c490: 6966 206d 2e67 6574 2827 536f 7274 4279  if m.get('SortBy
-0002c4a0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002c4b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002c4c0: 2e73 6f72 745f 6279 203d 206d 2e67 6574  .sort_by = m.get
-0002c4d0: 2827 536f 7274 4279 2729 0a20 2020 2020  ('SortBy').     
-0002c4e0: 2020 2069 6620 6d2e 6765 7428 2753 6f75     if m.get('Sou
-0002c4f0: 7263 6549 6427 2920 6973 206e 6f74 204e  rceId') is not N
-0002c500: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002c510: 2073 656c 662e 736f 7572 6365 5f69 6420   self.source_id 
-0002c520: 3d20 6d2e 6765 7428 2753 6f75 7263 6549  = m.get('SourceI
-0002c530: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-0002c540: 2e67 6574 2827 536f 7572 6365 5479 7065  .get('SourceType
-0002c550: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002c560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002c570: 2e73 6f75 7263 655f 7479 7065 203d 206d  .source_type = m
-0002c580: 2e67 6574 2827 536f 7572 6365 5479 7065  .get('SourceType
-0002c590: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0002c5a0: 6765 7428 2753 7461 7274 5469 6d65 2729  get('StartTime')
-0002c5b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002c5c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0002c5d0: 7461 7274 5f74 696d 6520 3d20 6d2e 6765  tart_time = m.ge
-0002c5e0: 7428 2753 7461 7274 5469 6d65 2729 0a20  t('StartTime'). 
-0002c5f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002c600: 2753 7461 7475 7327 2920 6973 206e 6f74  'Status') is not
-0002c610: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002c620: 2020 2073 656c 662e 7374 6174 7573 203d     self.status =
-0002c630: 206d 2e67 6574 2827 5374 6174 7573 2729   m.get('Status')
-0002c640: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002c650: 7428 2754 656e 736f 7262 6f61 7264 4964  t('TensorboardId
-0002c660: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002c670: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002c680: 2e74 656e 736f 7262 6f61 7264 5f69 6420  .tensorboard_id 
-0002c690: 3d20 6d2e 6765 7428 2754 656e 736f 7262  = m.get('Tensorb
-0002c6a0: 6f61 7264 4964 2729 0a20 2020 2020 2020  oardId').       
-0002c6b0: 2069 6620 6d2e 6765 7428 2756 6572 626f   if m.get('Verbo
-0002c6c0: 7365 2729 2069 7320 6e6f 7420 4e6f 6e65  se') is not None
-0002c6d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002c6e0: 6c66 2e76 6572 626f 7365 203d 206d 2e67  lf.verbose = m.g
-0002c6f0: 6574 2827 5665 7262 6f73 6527 290a 2020  et('Verbose').  
-0002c700: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002c710: 576f 726b 7370 6163 6549 6427 2920 6973  WorkspaceId') is
-0002c720: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002c730: 2020 2020 2020 2073 656c 662e 776f 726b         self.work
-0002c740: 7370 6163 655f 6964 203d 206d 2e67 6574  space_id = m.get
-0002c750: 2827 576f 726b 7370 6163 6549 6427 290a  ('WorkspaceId').
-0002c760: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0002c770: 656c 660a 0a0a 636c 6173 7320 4c69 7374  elf...class List
-0002c780: 5465 6e73 6f72 626f 6172 6473 5265 7370  TensorboardsResp
-0002c790: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
-0002c7a0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-0002c7b0: 6974 5f5f 2873 656c 662c 2072 6571 7565  it__(self, reque
-0002c7c0: 7374 5f69 643d 4e6f 6e65 2c20 7465 6e73  st_id=None, tens
-0002c7d0: 6f72 626f 6172 6473 3d4e 6f6e 652c 2074  orboards=None, t
-0002c7e0: 6f74 616c 5f63 6f75 6e74 3d4e 6f6e 6529  otal_count=None)
-0002c7f0: 3a0a 2020 2020 2020 2020 7365 6c66 2e72  :.        self.r
-0002c800: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
-0002c810: 6573 745f 6964 2020 2320 7479 7065 3a20  est_id  # type: 
-0002c820: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-0002c830: 2e74 656e 736f 7262 6f61 7264 7320 3d20  .tensorboards = 
-0002c840: 7465 6e73 6f72 626f 6172 6473 2020 2320  tensorboards  # 
-0002c850: 7479 7065 3a20 6c69 7374 5b54 656e 736f  type: list[Tenso
-0002c860: 7262 6f61 7264 5d0a 2020 2020 2020 2020  rboard].        
-0002c870: 7365 6c66 2e74 6f74 616c 5f63 6f75 6e74  self.total_count
-0002c880: 203d 2074 6f74 616c 5f63 6f75 6e74 2020   = total_count  
-0002c890: 2320 7479 7065 3a20 6c6f 6e67 0a0a 2020  # type: long..  
-0002c8a0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0002c8b0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
-0002c8c0: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
-0002c8d0: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
-0002c8e0: 666f 7220 6b20 696e 2073 656c 662e 7465  for k in self.te
-0002c8f0: 6e73 6f72 626f 6172 6473 3a0a 2020 2020  nsorboards:.    
-0002c900: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-0002c910: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002c920: 2020 2020 2020 6b2e 7661 6c69 6461 7465        k.validate
-0002c930: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-0002c940: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-0002c950: 2020 5f6d 6170 203d 2073 7570 6572 284c    _map = super(L
-0002c960: 6973 7454 656e 736f 7262 6f61 7264 7352  istTensorboardsR
-0002c970: 6573 706f 6e73 6542 6f64 792c 2073 656c  esponseBody, sel
-0002c980: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-0002c990: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0002c9a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002c9b0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0002c9c0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0002c9d0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0002c9e0: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-0002c9f0: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-0002ca00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002ca10: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
-0002ca20: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
-0002ca30: 5f69 640a 2020 2020 2020 2020 7265 7375  _id.        resu
-0002ca40: 6c74 5b27 5465 6e73 6f72 626f 6172 6473  lt['Tensorboards
-0002ca50: 275d 203d 205b 5d0a 2020 2020 2020 2020  '] = [].        
-0002ca60: 6966 2073 656c 662e 7465 6e73 6f72 626f  if self.tensorbo
-0002ca70: 6172 6473 2069 7320 6e6f 7420 4e6f 6e65  ards is not None
-0002ca80: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0002ca90: 7220 6b20 696e 2073 656c 662e 7465 6e73  r k in self.tens
-0002caa0: 6f72 626f 6172 6473 3a0a 2020 2020 2020  orboards:.      
+00026bf0: 6c66 0a0a 0a63 6c61 7373 2047 6574 546f  lf...class GetTo
+00026c00: 6b65 6e52 6571 7565 7374 2854 6561 4d6f  kenRequest(TeaMo
+00026c10: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+00026c20: 696e 6974 5f5f 2873 656c 662c 2065 7870  init__(self, exp
+00026c30: 6972 655f 7469 6d65 3d4e 6f6e 652c 2074  ire_time=None, t
+00026c40: 6172 6765 745f 6964 3d4e 6f6e 652c 2074  arget_id=None, t
+00026c50: 6172 6765 745f 7479 7065 3d4e 6f6e 6529  arget_type=None)
+00026c60: 3a0a 2020 2020 2020 2020 7365 6c66 2e65  :.        self.e
+00026c70: 7870 6972 655f 7469 6d65 203d 2065 7870  xpire_time = exp
+00026c80: 6972 655f 7469 6d65 2020 2320 7479 7065  ire_time  # type
+00026c90: 3a20 6c6f 6e67 0a20 2020 2020 2020 2073  : long.        s
+00026ca0: 656c 662e 7461 7267 6574 5f69 6420 3d20  elf.target_id = 
+00026cb0: 7461 7267 6574 5f69 6420 2023 2074 7970  target_id  # typ
+00026cc0: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+00026cd0: 656c 662e 7461 7267 6574 5f74 7970 6520  elf.target_type 
+00026ce0: 3d20 7461 7267 6574 5f74 7970 6520 2023  = target_type  #
+00026cf0: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
+00026d00: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00026d10: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+00026d20: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00026d30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00026d40: 5f6d 6170 203d 2073 7570 6572 2847 6574  _map = super(Get
+00026d50: 546f 6b65 6e52 6571 7565 7374 2c20 7365  TokenRequest, se
+00026d60: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+00026d70: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00026d80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00026d90: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00026da0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00026db0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00026dc0: 2020 2069 6620 7365 6c66 2e65 7870 6972     if self.expir
+00026dd0: 655f 7469 6d65 2069 7320 6e6f 7420 4e6f  e_time is not No
+00026de0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00026df0: 7265 7375 6c74 5b27 4578 7069 7265 5469  result['ExpireTi
+00026e00: 6d65 275d 203d 2073 656c 662e 6578 7069  me'] = self.expi
+00026e10: 7265 5f74 696d 650a 2020 2020 2020 2020  re_time.        
+00026e20: 6966 2073 656c 662e 7461 7267 6574 5f69  if self.target_i
+00026e30: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+00026e40: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00026e50: 745b 2754 6172 6765 7449 6427 5d20 3d20  t['TargetId'] = 
+00026e60: 7365 6c66 2e74 6172 6765 745f 6964 0a20  self.target_id. 
+00026e70: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00026e80: 6172 6765 745f 7479 7065 2069 7320 6e6f  arget_type is no
+00026e90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00026ea0: 2020 2020 7265 7375 6c74 5b27 5461 7267      result['Targ
+00026eb0: 6574 5479 7065 275d 203d 2073 656c 662e  etType'] = self.
+00026ec0: 7461 7267 6574 5f74 7970 650a 2020 2020  target_type.    
+00026ed0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00026ee0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+00026ef0: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
+00026f00: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+00026f10: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+00026f20: 2020 2069 6620 6d2e 6765 7428 2745 7870     if m.get('Exp
+00026f30: 6972 6554 696d 6527 2920 6973 206e 6f74  ireTime') is not
+00026f40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00026f50: 2020 2073 656c 662e 6578 7069 7265 5f74     self.expire_t
+00026f60: 696d 6520 3d20 6d2e 6765 7428 2745 7870  ime = m.get('Exp
+00026f70: 6972 6554 696d 6527 290a 2020 2020 2020  ireTime').      
+00026f80: 2020 6966 206d 2e67 6574 2827 5461 7267    if m.get('Targ
+00026f90: 6574 4964 2729 2069 7320 6e6f 7420 4e6f  etId') is not No
+00026fa0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00026fb0: 7365 6c66 2e74 6172 6765 745f 6964 203d  self.target_id =
+00026fc0: 206d 2e67 6574 2827 5461 7267 6574 4964   m.get('TargetId
+00026fd0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00026fe0: 6765 7428 2754 6172 6765 7454 7970 6527  get('TargetType'
+00026ff0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00027000: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00027010: 7461 7267 6574 5f74 7970 6520 3d20 6d2e  target_type = m.
+00027020: 6765 7428 2754 6172 6765 7454 7970 6527  get('TargetType'
+00027030: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00027040: 2073 656c 660a 0a0a 636c 6173 7320 4765   self...class Ge
+00027050: 7454 6f6b 656e 5265 7370 6f6e 7365 426f  tTokenResponseBo
+00027060: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
+00027070: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00027080: 656c 662c 2072 6571 7565 7374 5f69 643d  elf, request_id=
+00027090: 4e6f 6e65 2c20 746f 6b65 6e3d 4e6f 6e65  None, token=None
+000270a0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+000270b0: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
+000270c0: 7565 7374 5f69 6420 2023 2074 7970 653a  uest_id  # type:
+000270d0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+000270e0: 662e 746f 6b65 6e20 3d20 746f 6b65 6e20  f.token = token 
+000270f0: 2023 2074 7970 653a 2073 7472 0a0a 2020   # type: str..  
+00027100: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00027110: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+00027120: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+00027130: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00027140: 2020 5f6d 6170 203d 2073 7570 6572 2847    _map = super(G
+00027150: 6574 546f 6b65 6e52 6573 706f 6e73 6542  etTokenResponseB
+00027160: 6f64 792c 2073 656c 6629 2e74 6f5f 6d61  ody, self).to_ma
+00027170: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00027180: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00027190: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000271a0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+000271b0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+000271c0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+000271d0: 662e 7265 7175 6573 745f 6964 2069 7320  f.request_id is 
+000271e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000271f0: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
+00027200: 7175 6573 7449 6427 5d20 3d20 7365 6c66  questId'] = self
+00027210: 2e72 6571 7565 7374 5f69 640a 2020 2020  .request_id.    
+00027220: 2020 2020 6966 2073 656c 662e 746f 6b65      if self.toke
+00027230: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+00027240: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00027250: 745b 2754 6f6b 656e 275d 203d 2073 656c  t['Token'] = sel
+00027260: 662e 746f 6b65 6e0a 2020 2020 2020 2020  f.token.        
+00027270: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00027280: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00027290: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
+000272a0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+000272b0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000272c0: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
+000272d0: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+000272e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000272f0: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+00027300: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+00027310: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00027320: 6765 7428 2754 6f6b 656e 2729 2069 7320  get('Token') is 
+00027330: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00027340: 2020 2020 2020 7365 6c66 2e74 6f6b 656e        self.token
+00027350: 203d 206d 2e67 6574 2827 546f 6b65 6e27   = m.get('Token'
+00027360: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00027370: 2073 656c 660a 0a0a 636c 6173 7320 4765   self...class Ge
+00027380: 7454 6f6b 656e 5265 7370 6f6e 7365 2854  tTokenResponse(T
+00027390: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+000273a0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+000273b0: 2068 6561 6465 7273 3d4e 6f6e 652c 2073   headers=None, s
+000273c0: 7461 7475 735f 636f 6465 3d4e 6f6e 652c  tatus_code=None,
+000273d0: 2062 6f64 793d 4e6f 6e65 293a 0a20 2020   body=None):.   
+000273e0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+000273f0: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
+00027400: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
+00027410: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
+00027420: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+00027430: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
+00027440: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
+00027450: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+00027460: 2020 2320 7479 7065 3a20 4765 7454 6f6b    # type: GetTok
+00027470: 656e 5265 7370 6f6e 7365 426f 6479 0a0a  enResponseBody..
+00027480: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00027490: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000274a0: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+000274b0: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
+000274c0: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
+000274d0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+000274e0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+000274f0: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
+00027500: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
+00027510: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00027520: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+00027530: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
+00027540: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00027550: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+00027560: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+00027570: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+00027580: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00027590: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000275a0: 7570 6572 2847 6574 546f 6b65 6e52 6573  uper(GetTokenRes
+000275b0: 706f 6e73 652c 2073 656c 6629 2e74 6f5f  ponse, self).to_
+000275c0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000275d0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000275e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000275f0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00027600: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00027610: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00027620: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+00027630: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00027640: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+00027650: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+00027660: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+00027670: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00027680: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00027690: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000276a0: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+000276b0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+000276c0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+000276d0: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+000276e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000276f0: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+00027700: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+00027710: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+00027720: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00027730: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00027740: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+00027750: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00027760: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00027770: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
+00027780: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00027790: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+000277a0: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
+000277b0: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+000277c0: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
+000277d0: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
+000277e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000277f0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00027800: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
+00027810: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
+00027820: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
+00027830: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00027840: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+00027850: 6f64 656c 203d 2047 6574 546f 6b65 6e52  odel = GetTokenR
+00027860: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
+00027870: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00027880: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+00027890: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+000278a0: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+000278b0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+000278c0: 2047 6574 5765 6254 6572 6d69 6e61 6c52   GetWebTerminalR
+000278d0: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+000278e0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+000278f0: 5f5f 2873 656c 662c 2070 6f64 5f75 6964  __(self, pod_uid
+00027900: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00027910: 2320 506f 6420 5549 44e3 8082 0a20 2020  # Pod UID....   
+00027920: 2020 2020 2073 656c 662e 706f 645f 7569       self.pod_ui
+00027930: 6420 3d20 706f 645f 7569 6420 2023 2074  d = pod_uid  # t
+00027940: 7970 653a 2073 7472 0a0a 2020 2020 6465  ype: str..    de
+00027950: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00027960: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+00027970: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00027980: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+00027990: 6170 203d 2073 7570 6572 2847 6574 5765  ap = super(GetWe
+000279a0: 6254 6572 6d69 6e61 6c52 6571 7565 7374  bTerminalRequest
+000279b0: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+000279c0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+000279d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000279e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000279f0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00027a00: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00027a10: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00027a20: 6f64 5f75 6964 2069 7320 6e6f 7420 4e6f  od_uid is not No
+00027a30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00027a40: 7265 7375 6c74 5b27 506f 6455 6964 275d  result['PodUid']
+00027a50: 203d 2073 656c 662e 706f 645f 7569 640a   = self.pod_uid.
+00027a60: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00027a70: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00027a80: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+00027a90: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00027aa0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00027ab0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00027ac0: 2750 6f64 5569 6427 2920 6973 206e 6f74  'PodUid') is not
+00027ad0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00027ae0: 2020 2073 656c 662e 706f 645f 7569 6420     self.pod_uid 
+00027af0: 3d20 6d2e 6765 7428 2750 6f64 5569 6427  = m.get('PodUid'
+00027b00: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00027b10: 2073 656c 660a 0a0a 636c 6173 7320 4765   self...class Ge
+00027b20: 7457 6562 5465 726d 696e 616c 5265 7370  tWebTerminalResp
+00027b30: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
+00027b40: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00027b50: 6974 5f5f 2873 656c 662c 2072 6571 7565  it__(self, reque
+00027b60: 7374 5f69 643d 4e6f 6e65 2c20 7765 625f  st_id=None, web_
+00027b70: 7465 726d 696e 616c 5f75 726c 3d4e 6f6e  terminal_url=Non
+00027b80: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00027b90: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
+00027ba0: 7175 6573 745f 6964 2020 2320 7479 7065  quest_id  # type
+00027bb0: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
+00027bc0: 6c66 2e77 6562 5f74 6572 6d69 6e61 6c5f  lf.web_terminal_
+00027bd0: 7572 6c20 3d20 7765 625f 7465 726d 696e  url = web_termin
+00027be0: 616c 5f75 726c 2020 2320 7479 7065 3a20  al_url  # type: 
+00027bf0: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
+00027c00: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00027c10: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00027c20: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00027c30: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00027c40: 7375 7065 7228 4765 7457 6562 5465 726d  super(GetWebTerm
+00027c50: 696e 616c 5265 7370 6f6e 7365 426f 6479  inalResponseBody
+00027c60: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+00027c70: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00027c80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00027c90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00027ca0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00027cb0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00027cc0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00027cd0: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
+00027ce0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00027cf0: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
+00027d00: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
+00027d10: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+00027d20: 2069 6620 7365 6c66 2e77 6562 5f74 6572   if self.web_ter
+00027d30: 6d69 6e61 6c5f 7572 6c20 6973 206e 6f74  minal_url is not
+00027d40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00027d50: 2020 2072 6573 756c 745b 2757 6562 5465     result['WebTe
+00027d60: 726d 696e 616c 5572 6c27 5d20 3d20 7365  rminalUrl'] = se
+00027d70: 6c66 2e77 6562 5f74 6572 6d69 6e61 6c5f  lf.web_terminal_
+00027d80: 7572 6c0a 2020 2020 2020 2020 7265 7475  url.        retu
+00027d90: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00027da0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00027db0: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+00027dc0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00027dd0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00027de0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+00027df0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00027e00: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00027e10: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
+00027e20: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
+00027e30: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00027e40: 2757 6562 5465 726d 696e 616c 5572 6c27  'WebTerminalUrl'
+00027e50: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00027e60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00027e70: 7765 625f 7465 726d 696e 616c 5f75 726c  web_terminal_url
+00027e80: 203d 206d 2e67 6574 2827 5765 6254 6572   = m.get('WebTer
+00027e90: 6d69 6e61 6c55 726c 2729 0a20 2020 2020  minalUrl').     
+00027ea0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+00027eb0: 0a63 6c61 7373 2047 6574 5765 6254 6572  .class GetWebTer
+00027ec0: 6d69 6e61 6c52 6573 706f 6e73 6528 5465  minalResponse(Te
+00027ed0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00027ee0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00027ef0: 6865 6164 6572 733d 4e6f 6e65 2c20 7374  headers=None, st
+00027f00: 6174 7573 5f63 6f64 653d 4e6f 6e65 2c20  atus_code=None, 
+00027f10: 626f 6479 3d4e 6f6e 6529 3a0a 2020 2020  body=None):.    
+00027f20: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+00027f30: 203d 2068 6561 6465 7273 2020 2320 7479   = headers  # ty
+00027f40: 7065 3a20 6469 6374 5b73 7472 2c20 7374  pe: dict[str, st
+00027f50: 725d 0a20 2020 2020 2020 2073 656c 662e  r].        self.
+00027f60: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+00027f70: 6174 7573 5f63 6f64 6520 2023 2074 7970  atus_code  # typ
+00027f80: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
+00027f90: 656c 662e 626f 6479 203d 2062 6f64 7920  elf.body = body 
+00027fa0: 2023 2074 7970 653a 2047 6574 5765 6254   # type: GetWebT
+00027fb0: 6572 6d69 6e61 6c52 6573 706f 6e73 6542  erminalResponseB
+00027fc0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+00027fd0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00027fe0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+00027ff0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+00028000: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
+00028010: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
+00028020: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00028030: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
+00028040: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
+00028050: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
+00028060: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00028070: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
+00028080: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
+00028090: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
+000280a0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000280b0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
+000280c0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+000280d0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+000280e0: 7020 3d20 7375 7065 7228 4765 7457 6562  p = super(GetWeb
+000280f0: 5465 726d 696e 616c 5265 7370 6f6e 7365  TerminalResponse
+00028100: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+00028110: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00028120: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00028130: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00028140: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00028150: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00028160: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+00028170: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+00028180: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00028190: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+000281a0: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+000281b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000281c0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+000281d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000281e0: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+000281f0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+00028200: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+00028210: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+00028220: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+00028230: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00028240: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+00028250: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+00028260: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00028270: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00028280: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+00028290: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+000282a0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+000282b0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000282c0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+000282d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000282e0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000282f0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+00028300: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+00028310: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00028320: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00028330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00028340: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+00028350: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+00028360: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00028370: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+00028380: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00028390: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+000283a0: 3d20 4765 7457 6562 5465 726d 696e 616c  = GetWebTerminal
+000283b0: 5265 7370 6f6e 7365 426f 6479 2829 0a20  ResponseBody(). 
+000283c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000283d0: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+000283e0: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+000283f0: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+00028400: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00028410: 7320 4c69 7374 4563 7353 7065 6373 5265  s ListEcsSpecsRe
+00028420: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
+00028430: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00028440: 5f28 7365 6c66 2c20 6163 6365 6c65 7261  _(self, accelera
+00028450: 746f 725f 7479 7065 3d4e 6f6e 652c 206f  tor_type=None, o
+00028460: 7264 6572 3d4e 6f6e 652c 2070 6167 655f  rder=None, page_
+00028470: 6e75 6d62 6572 3d4e 6f6e 652c 2070 6167  number=None, pag
+00028480: 655f 7369 7a65 3d4e 6f6e 652c 2073 6f72  e_size=None, sor
+00028490: 745f 6279 3d4e 6f6e 6529 3a0a 2020 2020  t_by=None):.    
+000284a0: 2020 2020 7365 6c66 2e61 6363 656c 6572      self.acceler
+000284b0: 6174 6f72 5f74 7970 6520 3d20 6163 6365  ator_type = acce
+000284c0: 6c65 7261 746f 725f 7479 7065 2020 2320  lerator_type  # 
+000284d0: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
+000284e0: 2020 7365 6c66 2e6f 7264 6572 203d 206f    self.order = o
+000284f0: 7264 6572 2020 2320 7479 7065 3a20 7374  rder  # type: st
+00028500: 720a 2020 2020 2020 2020 7365 6c66 2e70  r.        self.p
+00028510: 6167 655f 6e75 6d62 6572 203d 2070 6167  age_number = pag
+00028520: 655f 6e75 6d62 6572 2020 2320 7479 7065  e_number  # type
+00028530: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
+00028540: 6c66 2e70 6167 655f 7369 7a65 203d 2070  lf.page_size = p
+00028550: 6167 655f 7369 7a65 2020 2320 7479 7065  age_size  # type
+00028560: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
+00028570: 6c66 2e73 6f72 745f 6279 203d 2073 6f72  lf.sort_by = sor
+00028580: 745f 6279 2020 2320 7479 7065 3a20 7374  t_by  # type: st
+00028590: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
+000285a0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+000285b0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+000285c0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000285d0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000285e0: 7065 7228 4c69 7374 4563 7353 7065 6373  per(ListEcsSpecs
+000285f0: 5265 7175 6573 742c 2073 656c 6629 2e74  Request, self).t
+00028600: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00028610: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00028620: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00028630: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00028640: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00028650: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00028660: 2073 656c 662e 6163 6365 6c65 7261 746f   self.accelerato
+00028670: 725f 7479 7065 2069 7320 6e6f 7420 4e6f  r_type is not No
+00028680: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00028690: 7265 7375 6c74 5b27 4163 6365 6c65 7261  result['Accelera
+000286a0: 746f 7254 7970 6527 5d20 3d20 7365 6c66  torType'] = self
+000286b0: 2e61 6363 656c 6572 6174 6f72 5f74 7970  .accelerator_typ
+000286c0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+000286d0: 662e 6f72 6465 7220 6973 206e 6f74 204e  f.order is not N
+000286e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000286f0: 2072 6573 756c 745b 274f 7264 6572 275d   result['Order']
+00028700: 203d 2073 656c 662e 6f72 6465 720a 2020   = self.order.  
+00028710: 2020 2020 2020 6966 2073 656c 662e 7061        if self.pa
+00028720: 6765 5f6e 756d 6265 7220 6973 206e 6f74  ge_number is not
+00028730: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00028740: 2020 2072 6573 756c 745b 2750 6167 654e     result['PageN
+00028750: 756d 6265 7227 5d20 3d20 7365 6c66 2e70  umber'] = self.p
+00028760: 6167 655f 6e75 6d62 6572 0a20 2020 2020  age_number.     
+00028770: 2020 2069 6620 7365 6c66 2e70 6167 655f     if self.page_
+00028780: 7369 7a65 2069 7320 6e6f 7420 4e6f 6e65  size is not None
+00028790: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000287a0: 7375 6c74 5b27 5061 6765 5369 7a65 275d  sult['PageSize']
+000287b0: 203d 2073 656c 662e 7061 6765 5f73 697a   = self.page_siz
+000287c0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+000287d0: 662e 736f 7274 5f62 7920 6973 206e 6f74  f.sort_by is not
+000287e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000287f0: 2020 2072 6573 756c 745b 2753 6f72 7442     result['SortB
+00028800: 7927 5d20 3d20 7365 6c66 2e73 6f72 745f  y'] = self.sort_
+00028810: 6279 0a20 2020 2020 2020 2072 6574 7572  by.        retur
+00028820: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+00028830: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+00028840: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+00028850: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+00028860: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00028870: 6574 2827 4163 6365 6c65 7261 746f 7254  et('AcceleratorT
+00028880: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
+00028890: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000288a0: 656c 662e 6163 6365 6c65 7261 746f 725f  elf.accelerator_
+000288b0: 7479 7065 203d 206d 2e67 6574 2827 4163  type = m.get('Ac
+000288c0: 6365 6c65 7261 746f 7254 7970 6527 290a  celeratorType').
+000288d0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000288e0: 2827 4f72 6465 7227 2920 6973 206e 6f74  ('Order') is not
+000288f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00028900: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
+00028910: 6d2e 6765 7428 274f 7264 6572 2729 0a20  m.get('Order'). 
+00028920: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00028930: 2750 6167 654e 756d 6265 7227 2920 6973  'PageNumber') is
+00028940: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00028950: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
+00028960: 5f6e 756d 6265 7220 3d20 6d2e 6765 7428  _number = m.get(
+00028970: 2750 6167 654e 756d 6265 7227 290a 2020  'PageNumber').  
+00028980: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00028990: 5061 6765 5369 7a65 2729 2069 7320 6e6f  PageSize') is no
+000289a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000289b0: 2020 2020 7365 6c66 2e70 6167 655f 7369      self.page_si
+000289c0: 7a65 203d 206d 2e67 6574 2827 5061 6765  ze = m.get('Page
+000289d0: 5369 7a65 2729 0a20 2020 2020 2020 2069  Size').        i
+000289e0: 6620 6d2e 6765 7428 2753 6f72 7442 7927  f m.get('SortBy'
+000289f0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00028a00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00028a10: 736f 7274 5f62 7920 3d20 6d2e 6765 7428  sort_by = m.get(
+00028a20: 2753 6f72 7442 7927 290a 2020 2020 2020  'SortBy').      
+00028a30: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00028a40: 636c 6173 7320 4c69 7374 4563 7353 7065  class ListEcsSpe
+00028a50: 6373 5265 7370 6f6e 7365 426f 6479 2854  csResponseBody(T
+00028a60: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00028a70: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00028a80: 2065 6373 5f73 7065 6373 3d4e 6f6e 652c   ecs_specs=None,
+00028a90: 2072 6571 7565 7374 5f69 643d 4e6f 6e65   request_id=None
+00028aa0: 2c20 746f 7461 6c5f 636f 756e 743d 4e6f  , total_count=No
+00028ab0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+00028ac0: 662e 6563 735f 7370 6563 7320 3d20 6563  f.ecs_specs = ec
+00028ad0: 735f 7370 6563 7320 2023 2074 7970 653a  s_specs  # type:
+00028ae0: 206c 6973 745b 4563 7353 7065 635d 0a20   list[EcsSpec]. 
+00028af0: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+00028b00: 6573 745f 6964 203d 2072 6571 7565 7374  est_id = request
+00028b10: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
+00028b20: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
+00028b30: 7461 6c5f 636f 756e 7420 3d20 746f 7461  tal_count = tota
+00028b40: 6c5f 636f 756e 7420 2023 2074 7970 653a  l_count  # type:
+00028b50: 206c 6f6e 670a 0a20 2020 2064 6566 2076   long..    def v
+00028b60: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00028b70: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+00028b80: 6373 5f73 7065 6373 3a0a 2020 2020 2020  cs_specs:.      
+00028b90: 2020 2020 2020 666f 7220 6b20 696e 2073        for k in s
+00028ba0: 656c 662e 6563 735f 7370 6563 733a 0a20  elf.ecs_specs:. 
+00028bb0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00028bc0: 6620 6b3a 0a20 2020 2020 2020 2020 2020  f k:.           
+00028bd0: 2020 2020 2020 2020 206b 2e76 616c 6964           k.valid
+00028be0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+00028bf0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00028c00: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00028c10: 7228 4c69 7374 4563 7353 7065 6373 5265  r(ListEcsSpecsRe
+00028c20: 7370 6f6e 7365 426f 6479 2c20 7365 6c66  sponseBody, self
+00028c30: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00028c40: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00028c50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00028c60: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00028c70: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00028c80: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00028c90: 2072 6573 756c 745b 2745 6373 5370 6563   result['EcsSpec
+00028ca0: 7327 5d20 3d20 5b5d 0a20 2020 2020 2020  s'] = [].       
+00028cb0: 2069 6620 7365 6c66 2e65 6373 5f73 7065   if self.ecs_spe
+00028cc0: 6373 2069 7320 6e6f 7420 4e6f 6e65 3a0a  cs is not None:.
+00028cd0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00028ce0: 6b20 696e 2073 656c 662e 6563 735f 7370  k in self.ecs_sp
+00028cf0: 6563 733a 0a20 2020 2020 2020 2020 2020  ecs:.           
+00028d00: 2020 2020 2072 6573 756c 745b 2745 6373       result['Ecs
+00028d10: 5370 6563 7327 5d2e 6170 7065 6e64 286b  Specs'].append(k
+00028d20: 2e74 6f5f 6d61 7028 2920 6966 206b 2065  .to_map() if k e
+00028d30: 6c73 6520 4e6f 6e65 290a 2020 2020 2020  lse None).      
+00028d40: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
+00028d50: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
+00028d60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00028d70: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
+00028d80: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
+00028d90: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00028da0: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
+00028db0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00028dc0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00028dd0: 2754 6f74 616c 436f 756e 7427 5d20 3d20  'TotalCount'] = 
+00028de0: 7365 6c66 2e74 6f74 616c 5f63 6f75 6e74  self.total_count
+00028df0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00028e00: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00028e10: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00028e20: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00028e30: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00028e40: 2020 2020 2020 2020 7365 6c66 2e65 6373          self.ecs
+00028e50: 5f73 7065 6373 203d 205b 5d0a 2020 2020  _specs = [].    
+00028e60: 2020 2020 6966 206d 2e67 6574 2827 4563      if m.get('Ec
+00028e70: 7353 7065 6373 2729 2069 7320 6e6f 7420  sSpecs') is not 
+00028e80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00028e90: 2020 666f 7220 6b20 696e 206d 2e67 6574    for k in m.get
+00028ea0: 2827 4563 7353 7065 6373 2729 3a0a 2020  ('EcsSpecs'):.  
+00028eb0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00028ec0: 6d70 5f6d 6f64 656c 203d 2045 6373 5370  mp_model = EcsSp
+00028ed0: 6563 2829 0a20 2020 2020 2020 2020 2020  ec().           
+00028ee0: 2020 2020 2073 656c 662e 6563 735f 7370       self.ecs_sp
+00028ef0: 6563 732e 6170 7065 6e64 2874 656d 705f  ecs.append(temp_
+00028f00: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286b  model.from_map(k
+00028f10: 2929 0a20 2020 2020 2020 2069 6620 6d2e  )).        if m.
+00028f20: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+00028f30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00028f40: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00028f50: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
+00028f60: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
+00028f70: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00028f80: 2754 6f74 616c 436f 756e 7427 2920 6973  'TotalCount') is
+00028f90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00028fa0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
+00028fb0: 6c5f 636f 756e 7420 3d20 6d2e 6765 7428  l_count = m.get(
+00028fc0: 2754 6f74 616c 436f 756e 7427 290a 2020  'TotalCount').  
+00028fd0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00028fe0: 660a 0a0a 636c 6173 7320 4c69 7374 4563  f...class ListEc
+00028ff0: 7353 7065 6373 5265 7370 6f6e 7365 2854  sSpecsResponse(T
+00029000: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00029010: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00029020: 2068 6561 6465 7273 3d4e 6f6e 652c 2073   headers=None, s
+00029030: 7461 7475 735f 636f 6465 3d4e 6f6e 652c  tatus_code=None,
+00029040: 2062 6f64 793d 4e6f 6e65 293a 0a20 2020   body=None):.   
+00029050: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00029060: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
+00029070: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
+00029080: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
+00029090: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+000290a0: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
+000290b0: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
+000290c0: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+000290d0: 2020 2320 7479 7065 3a20 4c69 7374 4563    # type: ListEc
+000290e0: 7353 7065 6373 5265 7370 6f6e 7365 426f  sSpecsResponseBo
+000290f0: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
+00029100: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00029110: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+00029120: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+00029130: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
+00029140: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
+00029150: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+00029160: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
+00029170: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
+00029180: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
+00029190: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+000291a0: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
+000291b0: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
+000291c0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+000291d0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+000291e0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+000291f0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00029200: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00029210: 203d 2073 7570 6572 284c 6973 7445 6373   = super(ListEcs
+00029220: 5370 6563 7352 6573 706f 6e73 652c 2073  SpecsResponse, s
+00029230: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
+00029240: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00029250: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00029260: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00029270: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00029280: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00029290: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
+000292a0: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
+000292b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000292c0: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
+000292d0: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
+000292e0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+000292f0: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
+00029300: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00029310: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
+00029320: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
+00029330: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+00029340: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
+00029350: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00029360: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00029370: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
+00029380: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
+00029390: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000293a0: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+000293b0: 5f6d 6170 2873 656c 662c 206d 3d4e 6f6e  _map(self, m=Non
+000293c0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+000293d0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+000293e0: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+000293f0: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+00029400: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00029410: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+00029420: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00029430: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00029440: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+00029450: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00029460: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00029470: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+00029480: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+00029490: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000294a0: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+000294b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000294c0: 2020 7465 6d70 5f6d 6f64 656c 203d 204c    temp_model = L
+000294d0: 6973 7445 6373 5370 6563 7352 6573 706f  istEcsSpecsRespo
+000294e0: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
+000294f0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00029500: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+00029510: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+00029520: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00029530: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
+00029540: 744a 6f62 7352 6571 7565 7374 2854 6561  tJobsRequest(Tea
+00029550: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+00029560: 5f5f 696e 6974 5f5f 2873 656c 662c 2062  __init__(self, b
+00029570: 7573 696e 6573 735f 7573 6572 5f69 643d  usiness_user_id=
+00029580: 4e6f 6e65 2c20 6361 6c6c 6572 3d4e 6f6e  None, caller=Non
+00029590: 652c 2064 6973 706c 6179 5f6e 616d 653d  e, display_name=
+000295a0: 4e6f 6e65 2c20 656e 645f 7469 6d65 3d4e  None, end_time=N
+000295b0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+000295c0: 2020 2020 2020 6672 6f6d 5f61 6c6c 5f77        from_all_w
+000295d0: 6f72 6b73 7061 6365 733d 4e6f 6e65 2c20  orkspaces=None, 
+000295e0: 6a6f 625f 6964 3d4e 6f6e 652c 206a 6f62  job_id=None, job
+000295f0: 5f74 7970 653d 4e6f 6e65 2c20 6f72 6465  _type=None, orde
+00029600: 723d 4e6f 6e65 2c20 7061 6765 5f6e 756d  r=None, page_num
+00029610: 6265 723d 4e6f 6e65 2c20 7061 6765 5f73  ber=None, page_s
+00029620: 697a 653d 4e6f 6e65 2c20 7069 7065 6c69  ize=None, pipeli
+00029630: 6e65 5f69 643d 4e6f 6e65 2c0a 2020 2020  ne_id=None,.    
+00029640: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00029650: 6f75 7263 655f 6964 3d4e 6f6e 652c 2073  ource_id=None, s
+00029660: 686f 775f 6f77 6e3d 4e6f 6e65 2c20 736f  how_own=None, so
+00029670: 7274 5f62 793d 4e6f 6e65 2c20 7374 6172  rt_by=None, star
+00029680: 745f 7469 6d65 3d4e 6f6e 652c 2073 7461  t_time=None, sta
+00029690: 7475 733d 4e6f 6e65 2c20 7461 6773 3d4e  tus=None, tags=N
+000296a0: 6f6e 652c 2077 6f72 6b73 7061 6365 5f69  one, workspace_i
+000296b0: 643d 4e6f 6e65 293a 0a20 2020 2020 2020  d=None):.       
+000296c0: 2073 656c 662e 6275 7369 6e65 7373 5f75   self.business_u
+000296d0: 7365 725f 6964 203d 2062 7573 696e 6573  ser_id = busines
+000296e0: 735f 7573 6572 5f69 6420 2023 2074 7970  s_user_id  # typ
+000296f0: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+00029700: 656c 662e 6361 6c6c 6572 203d 2063 616c  elf.caller = cal
+00029710: 6c65 7220 2023 2074 7970 653a 2073 7472  ler  # type: str
+00029720: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
+00029730: 7370 6c61 795f 6e61 6d65 203d 2064 6973  splay_name = dis
+00029740: 706c 6179 5f6e 616d 6520 2023 2074 7970  play_name  # typ
+00029750: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+00029760: 656c 662e 656e 645f 7469 6d65 203d 2065  elf.end_time = e
+00029770: 6e64 5f74 696d 6520 2023 2074 7970 653a  nd_time  # type:
+00029780: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00029790: 662e 6672 6f6d 5f61 6c6c 5f77 6f72 6b73  f.from_all_works
+000297a0: 7061 6365 7320 3d20 6672 6f6d 5f61 6c6c  paces = from_all
+000297b0: 5f77 6f72 6b73 7061 6365 7320 2023 2074  _workspaces  # t
+000297c0: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+000297d0: 2020 7365 6c66 2e6a 6f62 5f69 6420 3d20    self.job_id = 
+000297e0: 6a6f 625f 6964 2020 2320 7479 7065 3a20  job_id  # type: 
+000297f0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+00029800: 2e6a 6f62 5f74 7970 6520 3d20 6a6f 625f  .job_type = job_
+00029810: 7479 7065 2020 2320 7479 7065 3a20 7374  type  # type: st
+00029820: 720a 2020 2020 2020 2020 7365 6c66 2e6f  r.        self.o
+00029830: 7264 6572 203d 206f 7264 6572 2020 2320  rder = order  # 
+00029840: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
+00029850: 2020 7365 6c66 2e70 6167 655f 6e75 6d62    self.page_numb
+00029860: 6572 203d 2070 6167 655f 6e75 6d62 6572  er = page_number
+00029870: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
+00029880: 2020 2020 2020 7365 6c66 2e70 6167 655f        self.page_
+00029890: 7369 7a65 203d 2070 6167 655f 7369 7a65  size = page_size
+000298a0: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
+000298b0: 2020 2020 2020 7365 6c66 2e70 6970 656c        self.pipel
+000298c0: 696e 655f 6964 203d 2070 6970 656c 696e  ine_id = pipelin
+000298d0: 655f 6964 2020 2320 7479 7065 3a20 7374  e_id  # type: st
+000298e0: 720a 2020 2020 2020 2020 7365 6c66 2e72  r.        self.r
+000298f0: 6573 6f75 7263 655f 6964 203d 2072 6573  esource_id = res
+00029900: 6f75 7263 655f 6964 2020 2320 7479 7065  ource_id  # type
+00029910: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
+00029920: 6c66 2e73 686f 775f 6f77 6e20 3d20 7368  lf.show_own = sh
+00029930: 6f77 5f6f 776e 2020 2320 7479 7065 3a20  ow_own  # type: 
+00029940: 626f 6f6c 0a20 2020 2020 2020 2073 656c  bool.        sel
+00029950: 662e 736f 7274 5f62 7920 3d20 736f 7274  f.sort_by = sort
+00029960: 5f62 7920 2023 2074 7970 653a 2073 7472  _by  # type: str
+00029970: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00029980: 6172 745f 7469 6d65 203d 2073 7461 7274  art_time = start
+00029990: 5f74 696d 6520 2023 2074 7970 653a 2073  _time  # type: s
+000299a0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+000299b0: 7374 6174 7573 203d 2073 7461 7475 7320  status = status 
+000299c0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+000299d0: 2020 2020 2073 656c 662e 7461 6773 203d       self.tags =
+000299e0: 2074 6167 7320 2023 2074 7970 653a 2064   tags  # type: d
+000299f0: 6963 745b 7374 722c 2073 7472 5d0a 2020  ict[str, str].  
+00029a00: 2020 2020 2020 7365 6c66 2e77 6f72 6b73        self.works
+00029a10: 7061 6365 5f69 6420 3d20 776f 726b 7370  pace_id = worksp
+00029a20: 6163 655f 6964 2020 2320 7479 7065 3a20  ace_id  # type: 
+00029a30: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
+00029a40: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00029a50: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00029a60: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00029a70: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00029a80: 7375 7065 7228 4c69 7374 4a6f 6273 5265  super(ListJobsRe
+00029a90: 7175 6573 742c 2073 656c 6629 2e74 6f5f  quest, self).to_
+00029aa0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00029ab0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00029ac0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00029ad0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00029ae0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00029af0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00029b00: 656c 662e 6275 7369 6e65 7373 5f75 7365  elf.business_use
+00029b10: 725f 6964 2069 7320 6e6f 7420 4e6f 6e65  r_id is not None
+00029b20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00029b30: 7375 6c74 5b27 4275 7369 6e65 7373 5573  sult['BusinessUs
+00029b40: 6572 4964 275d 203d 2073 656c 662e 6275  erId'] = self.bu
+00029b50: 7369 6e65 7373 5f75 7365 725f 6964 0a20  siness_user_id. 
+00029b60: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00029b70: 616c 6c65 7220 6973 206e 6f74 204e 6f6e  aller is not Non
+00029b80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00029b90: 6573 756c 745b 2743 616c 6c65 7227 5d20  esult['Caller'] 
+00029ba0: 3d20 7365 6c66 2e63 616c 6c65 720a 2020  = self.caller.  
+00029bb0: 2020 2020 2020 6966 2073 656c 662e 6469        if self.di
+00029bc0: 7370 6c61 795f 6e61 6d65 2069 7320 6e6f  splay_name is no
+00029bd0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00029be0: 2020 2020 7265 7375 6c74 5b27 4469 7370      result['Disp
+00029bf0: 6c61 794e 616d 6527 5d20 3d20 7365 6c66  layName'] = self
+00029c00: 2e64 6973 706c 6179 5f6e 616d 650a 2020  .display_name.  
+00029c10: 2020 2020 2020 6966 2073 656c 662e 656e        if self.en
+00029c20: 645f 7469 6d65 2069 7320 6e6f 7420 4e6f  d_time is not No
+00029c30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00029c40: 7265 7375 6c74 5b27 456e 6454 696d 6527  result['EndTime'
+00029c50: 5d20 3d20 7365 6c66 2e65 6e64 5f74 696d  ] = self.end_tim
+00029c60: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00029c70: 662e 6672 6f6d 5f61 6c6c 5f77 6f72 6b73  f.from_all_works
+00029c80: 7061 6365 7320 6973 206e 6f74 204e 6f6e  paces is not Non
+00029c90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00029ca0: 6573 756c 745b 2746 726f 6d41 6c6c 576f  esult['FromAllWo
+00029cb0: 726b 7370 6163 6573 275d 203d 2073 656c  rkspaces'] = sel
+00029cc0: 662e 6672 6f6d 5f61 6c6c 5f77 6f72 6b73  f.from_all_works
+00029cd0: 7061 6365 730a 2020 2020 2020 2020 6966  paces.        if
+00029ce0: 2073 656c 662e 6a6f 625f 6964 2069 7320   self.job_id is 
+00029cf0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00029d00: 2020 2020 2020 7265 7375 6c74 5b27 4a6f        result['Jo
+00029d10: 6249 6427 5d20 3d20 7365 6c66 2e6a 6f62  bId'] = self.job
+00029d20: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00029d30: 656c 662e 6a6f 625f 7479 7065 2069 7320  elf.job_type is 
+00029d40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00029d50: 2020 2020 2020 7265 7375 6c74 5b27 4a6f        result['Jo
+00029d60: 6254 7970 6527 5d20 3d20 7365 6c66 2e6a  bType'] = self.j
+00029d70: 6f62 5f74 7970 650a 2020 2020 2020 2020  ob_type.        
+00029d80: 6966 2073 656c 662e 6f72 6465 7220 6973  if self.order is
+00029d90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00029da0: 2020 2020 2020 2072 6573 756c 745b 274f         result['O
+00029db0: 7264 6572 275d 203d 2073 656c 662e 6f72  rder'] = self.or
+00029dc0: 6465 720a 2020 2020 2020 2020 6966 2073  der.        if s
+00029dd0: 656c 662e 7061 6765 5f6e 756d 6265 7220  elf.page_number 
+00029de0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00029df0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00029e00: 2750 6167 654e 756d 6265 7227 5d20 3d20  'PageNumber'] = 
+00029e10: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
+00029e20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00029e30: 2e70 6167 655f 7369 7a65 2069 7320 6e6f  .page_size is no
+00029e40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00029e50: 2020 2020 7265 7375 6c74 5b27 5061 6765      result['Page
+00029e60: 5369 7a65 275d 203d 2073 656c 662e 7061  Size'] = self.pa
+00029e70: 6765 5f73 697a 650a 2020 2020 2020 2020  ge_size.        
+00029e80: 6966 2073 656c 662e 7069 7065 6c69 6e65  if self.pipeline
+00029e90: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00029ea0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00029eb0: 756c 745b 2750 6970 656c 696e 6549 6427  ult['PipelineId'
+00029ec0: 5d20 3d20 7365 6c66 2e70 6970 656c 696e  ] = self.pipelin
+00029ed0: 655f 6964 0a20 2020 2020 2020 2069 6620  e_id.        if 
+00029ee0: 7365 6c66 2e72 6573 6f75 7263 655f 6964  self.resource_id
+00029ef0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00029f00: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00029f10: 5b27 5265 736f 7572 6365 4964 275d 203d  ['ResourceId'] =
+00029f20: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
+00029f30: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+00029f40: 662e 7368 6f77 5f6f 776e 2069 7320 6e6f  f.show_own is no
+00029f50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00029f60: 2020 2020 7265 7375 6c74 5b27 5368 6f77      result['Show
+00029f70: 4f77 6e27 5d20 3d20 7365 6c66 2e73 686f  Own'] = self.sho
+00029f80: 775f 6f77 6e0a 2020 2020 2020 2020 6966  w_own.        if
+00029f90: 2073 656c 662e 736f 7274 5f62 7920 6973   self.sort_by is
+00029fa0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00029fb0: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
+00029fc0: 6f72 7442 7927 5d20 3d20 7365 6c66 2e73  ortBy'] = self.s
+00029fd0: 6f72 745f 6279 0a20 2020 2020 2020 2069  ort_by.        i
+00029fe0: 6620 7365 6c66 2e73 7461 7274 5f74 696d  f self.start_tim
+00029ff0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+0002a000: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002a010: 745b 2753 7461 7274 5469 6d65 275d 203d  t['StartTime'] =
+0002a020: 2073 656c 662e 7374 6172 745f 7469 6d65   self.start_time
+0002a030: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002a040: 2e73 7461 7475 7320 6973 206e 6f74 204e  .status is not N
+0002a050: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002a060: 2072 6573 756c 745b 2753 7461 7475 7327   result['Status'
+0002a070: 5d20 3d20 7365 6c66 2e73 7461 7475 730a  ] = self.status.
+0002a080: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002a090: 7461 6773 2069 7320 6e6f 7420 4e6f 6e65  tags is not None
+0002a0a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002a0b0: 7375 6c74 5b27 5461 6773 275d 203d 2073  sult['Tags'] = s
+0002a0c0: 656c 662e 7461 6773 0a20 2020 2020 2020  elf.tags.       
+0002a0d0: 2069 6620 7365 6c66 2e77 6f72 6b73 7061   if self.workspa
+0002a0e0: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
+0002a0f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002a100: 6573 756c 745b 2757 6f72 6b73 7061 6365  esult['Workspace
+0002a110: 4964 275d 203d 2073 656c 662e 776f 726b  Id'] = self.work
+0002a120: 7370 6163 655f 6964 0a20 2020 2020 2020  space_id.       
+0002a130: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0002a140: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+0002a150: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+0002a160: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0002a170: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0002a180: 6966 206d 2e67 6574 2827 4275 7369 6e65  if m.get('Busine
+0002a190: 7373 5573 6572 4964 2729 2069 7320 6e6f  ssUserId') is no
+0002a1a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002a1b0: 2020 2020 7365 6c66 2e62 7573 696e 6573      self.busines
+0002a1c0: 735f 7573 6572 5f69 6420 3d20 6d2e 6765  s_user_id = m.ge
+0002a1d0: 7428 2742 7573 696e 6573 7355 7365 7249  t('BusinessUserI
+0002a1e0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+0002a1f0: 2e67 6574 2827 4361 6c6c 6572 2729 2069  .get('Caller') i
+0002a200: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002a210: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
+0002a220: 6c65 7220 3d20 6d2e 6765 7428 2743 616c  ler = m.get('Cal
+0002a230: 6c65 7227 290a 2020 2020 2020 2020 6966  ler').        if
+0002a240: 206d 2e67 6574 2827 4469 7370 6c61 794e   m.get('DisplayN
+0002a250: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
+0002a260: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002a270: 656c 662e 6469 7370 6c61 795f 6e61 6d65  elf.display_name
+0002a280: 203d 206d 2e67 6574 2827 4469 7370 6c61   = m.get('Displa
+0002a290: 794e 616d 6527 290a 2020 2020 2020 2020  yName').        
+0002a2a0: 6966 206d 2e67 6574 2827 456e 6454 696d  if m.get('EndTim
+0002a2b0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+0002a2c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002a2d0: 662e 656e 645f 7469 6d65 203d 206d 2e67  f.end_time = m.g
+0002a2e0: 6574 2827 456e 6454 696d 6527 290a 2020  et('EndTime').  
+0002a2f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002a300: 4672 6f6d 416c 6c57 6f72 6b73 7061 6365  FromAllWorkspace
+0002a310: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+0002a320: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002a330: 662e 6672 6f6d 5f61 6c6c 5f77 6f72 6b73  f.from_all_works
+0002a340: 7061 6365 7320 3d20 6d2e 6765 7428 2746  paces = m.get('F
+0002a350: 726f 6d41 6c6c 576f 726b 7370 6163 6573  romAllWorkspaces
+0002a360: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002a370: 6765 7428 274a 6f62 4964 2729 2069 7320  get('JobId') is 
+0002a380: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002a390: 2020 2020 2020 7365 6c66 2e6a 6f62 5f69        self.job_i
+0002a3a0: 6420 3d20 6d2e 6765 7428 274a 6f62 4964  d = m.get('JobId
+0002a3b0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002a3c0: 6765 7428 274a 6f62 5479 7065 2729 2069  get('JobType') i
+0002a3d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002a3e0: 2020 2020 2020 2020 7365 6c66 2e6a 6f62          self.job
+0002a3f0: 5f74 7970 6520 3d20 6d2e 6765 7428 274a  _type = m.get('J
+0002a400: 6f62 5479 7065 2729 0a20 2020 2020 2020  obType').       
+0002a410: 2069 6620 6d2e 6765 7428 274f 7264 6572   if m.get('Order
+0002a420: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0002a430: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002a440: 2e6f 7264 6572 203d 206d 2e67 6574 2827  .order = m.get('
+0002a450: 4f72 6465 7227 290a 2020 2020 2020 2020  Order').        
+0002a460: 6966 206d 2e67 6574 2827 5061 6765 4e75  if m.get('PageNu
+0002a470: 6d62 6572 2729 2069 7320 6e6f 7420 4e6f  mber') is not No
+0002a480: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002a490: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
+0002a4a0: 203d 206d 2e67 6574 2827 5061 6765 4e75   = m.get('PageNu
+0002a4b0: 6d62 6572 2729 0a20 2020 2020 2020 2069  mber').        i
+0002a4c0: 6620 6d2e 6765 7428 2750 6167 6553 697a  f m.get('PageSiz
+0002a4d0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+0002a4e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002a4f0: 662e 7061 6765 5f73 697a 6520 3d20 6d2e  f.page_size = m.
+0002a500: 6765 7428 2750 6167 6553 697a 6527 290a  get('PageSize').
+0002a510: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002a520: 2827 5069 7065 6c69 6e65 4964 2729 2069  ('PipelineId') i
+0002a530: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002a540: 2020 2020 2020 2020 7365 6c66 2e70 6970          self.pip
+0002a550: 656c 696e 655f 6964 203d 206d 2e67 6574  eline_id = m.get
+0002a560: 2827 5069 7065 6c69 6e65 4964 2729 0a20  ('PipelineId'). 
+0002a570: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002a580: 2752 6573 6f75 7263 6549 6427 2920 6973  'ResourceId') is
+0002a590: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002a5a0: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
+0002a5b0: 7572 6365 5f69 6420 3d20 6d2e 6765 7428  urce_id = m.get(
+0002a5c0: 2752 6573 6f75 7263 6549 6427 290a 2020  'ResourceId').  
+0002a5d0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002a5e0: 5368 6f77 4f77 6e27 2920 6973 206e 6f74  ShowOwn') is not
+0002a5f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002a600: 2020 2073 656c 662e 7368 6f77 5f6f 776e     self.show_own
+0002a610: 203d 206d 2e67 6574 2827 5368 6f77 4f77   = m.get('ShowOw
+0002a620: 6e27 290a 2020 2020 2020 2020 6966 206d  n').        if m
+0002a630: 2e67 6574 2827 536f 7274 4279 2729 2069  .get('SortBy') i
+0002a640: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002a650: 2020 2020 2020 2020 7365 6c66 2e73 6f72          self.sor
+0002a660: 745f 6279 203d 206d 2e67 6574 2827 536f  t_by = m.get('So
+0002a670: 7274 4279 2729 0a20 2020 2020 2020 2069  rtBy').        i
+0002a680: 6620 6d2e 6765 7428 2753 7461 7274 5469  f m.get('StartTi
+0002a690: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
+0002a6a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002a6b0: 6c66 2e73 7461 7274 5f74 696d 6520 3d20  lf.start_time = 
+0002a6c0: 6d2e 6765 7428 2753 7461 7274 5469 6d65  m.get('StartTime
+0002a6d0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002a6e0: 6765 7428 2753 7461 7475 7327 2920 6973  get('Status') is
+0002a6f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002a700: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0002a710: 7573 203d 206d 2e67 6574 2827 5374 6174  us = m.get('Stat
+0002a720: 7573 2729 0a20 2020 2020 2020 2069 6620  us').        if 
+0002a730: 6d2e 6765 7428 2754 6167 7327 2920 6973  m.get('Tags') is
+0002a740: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002a750: 2020 2020 2020 2073 656c 662e 7461 6773         self.tags
+0002a760: 203d 206d 2e67 6574 2827 5461 6773 2729   = m.get('Tags')
+0002a770: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002a780: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
+0002a790: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a7a0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+0002a7b0: 6f72 6b73 7061 6365 5f69 6420 3d20 6d2e  orkspace_id = m.
+0002a7c0: 6765 7428 2757 6f72 6b73 7061 6365 4964  get('WorkspaceId
+0002a7d0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+0002a7e0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
+0002a7f0: 6973 744a 6f62 7353 6872 696e 6b52 6571  istJobsShrinkReq
+0002a800: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+0002a810: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0002a820: 2873 656c 662c 2062 7573 696e 6573 735f  (self, business_
+0002a830: 7573 6572 5f69 643d 4e6f 6e65 2c20 6361  user_id=None, ca
+0002a840: 6c6c 6572 3d4e 6f6e 652c 2064 6973 706c  ller=None, displ
+0002a850: 6179 5f6e 616d 653d 4e6f 6e65 2c20 656e  ay_name=None, en
+0002a860: 645f 7469 6d65 3d4e 6f6e 652c 0a20 2020  d_time=None,.   
+0002a870: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+0002a880: 6f6d 5f61 6c6c 5f77 6f72 6b73 7061 6365  om_all_workspace
+0002a890: 733d 4e6f 6e65 2c20 6a6f 625f 6964 3d4e  s=None, job_id=N
+0002a8a0: 6f6e 652c 206a 6f62 5f74 7970 653d 4e6f  one, job_type=No
+0002a8b0: 6e65 2c20 6f72 6465 723d 4e6f 6e65 2c20  ne, order=None, 
+0002a8c0: 7061 6765 5f6e 756d 6265 723d 4e6f 6e65  page_number=None
+0002a8d0: 2c20 7061 6765 5f73 697a 653d 4e6f 6e65  , page_size=None
+0002a8e0: 2c20 7069 7065 6c69 6e65 5f69 643d 4e6f  , pipeline_id=No
+0002a8f0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0002a900: 2020 2020 2072 6573 6f75 7263 655f 6964       resource_id
+0002a910: 3d4e 6f6e 652c 2073 686f 775f 6f77 6e3d  =None, show_own=
+0002a920: 4e6f 6e65 2c20 736f 7274 5f62 793d 4e6f  None, sort_by=No
+0002a930: 6e65 2c20 7374 6172 745f 7469 6d65 3d4e  ne, start_time=N
+0002a940: 6f6e 652c 2073 7461 7475 733d 4e6f 6e65  one, status=None
+0002a950: 2c20 7461 6773 5f73 6872 696e 6b3d 4e6f  , tags_shrink=No
+0002a960: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0002a970: 2020 2020 2077 6f72 6b73 7061 6365 5f69       workspace_i
+0002a980: 643d 4e6f 6e65 293a 0a20 2020 2020 2020  d=None):.       
+0002a990: 2073 656c 662e 6275 7369 6e65 7373 5f75   self.business_u
+0002a9a0: 7365 725f 6964 203d 2062 7573 696e 6573  ser_id = busines
+0002a9b0: 735f 7573 6572 5f69 6420 2023 2074 7970  s_user_id  # typ
+0002a9c0: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+0002a9d0: 656c 662e 6361 6c6c 6572 203d 2063 616c  elf.caller = cal
+0002a9e0: 6c65 7220 2023 2074 7970 653a 2073 7472  ler  # type: str
+0002a9f0: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
+0002aa00: 7370 6c61 795f 6e61 6d65 203d 2064 6973  splay_name = dis
+0002aa10: 706c 6179 5f6e 616d 6520 2023 2074 7970  play_name  # typ
+0002aa20: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+0002aa30: 656c 662e 656e 645f 7469 6d65 203d 2065  elf.end_time = e
+0002aa40: 6e64 5f74 696d 6520 2023 2074 7970 653a  nd_time  # type:
+0002aa50: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0002aa60: 662e 6672 6f6d 5f61 6c6c 5f77 6f72 6b73  f.from_all_works
+0002aa70: 7061 6365 7320 3d20 6672 6f6d 5f61 6c6c  paces = from_all
+0002aa80: 5f77 6f72 6b73 7061 6365 7320 2023 2074  _workspaces  # t
+0002aa90: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+0002aaa0: 2020 7365 6c66 2e6a 6f62 5f69 6420 3d20    self.job_id = 
+0002aab0: 6a6f 625f 6964 2020 2320 7479 7065 3a20  job_id  # type: 
+0002aac0: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+0002aad0: 2e6a 6f62 5f74 7970 6520 3d20 6a6f 625f  .job_type = job_
+0002aae0: 7479 7065 2020 2320 7479 7065 3a20 7374  type  # type: st
+0002aaf0: 720a 2020 2020 2020 2020 7365 6c66 2e6f  r.        self.o
+0002ab00: 7264 6572 203d 206f 7264 6572 2020 2320  rder = order  # 
+0002ab10: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
+0002ab20: 2020 7365 6c66 2e70 6167 655f 6e75 6d62    self.page_numb
+0002ab30: 6572 203d 2070 6167 655f 6e75 6d62 6572  er = page_number
+0002ab40: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
+0002ab50: 2020 2020 2020 7365 6c66 2e70 6167 655f        self.page_
+0002ab60: 7369 7a65 203d 2070 6167 655f 7369 7a65  size = page_size
+0002ab70: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
+0002ab80: 2020 2020 2020 7365 6c66 2e70 6970 656c        self.pipel
+0002ab90: 696e 655f 6964 203d 2070 6970 656c 696e  ine_id = pipelin
+0002aba0: 655f 6964 2020 2320 7479 7065 3a20 7374  e_id  # type: st
+0002abb0: 720a 2020 2020 2020 2020 7365 6c66 2e72  r.        self.r
+0002abc0: 6573 6f75 7263 655f 6964 203d 2072 6573  esource_id = res
+0002abd0: 6f75 7263 655f 6964 2020 2320 7479 7065  ource_id  # type
+0002abe0: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
+0002abf0: 6c66 2e73 686f 775f 6f77 6e20 3d20 7368  lf.show_own = sh
+0002ac00: 6f77 5f6f 776e 2020 2320 7479 7065 3a20  ow_own  # type: 
+0002ac10: 626f 6f6c 0a20 2020 2020 2020 2073 656c  bool.        sel
+0002ac20: 662e 736f 7274 5f62 7920 3d20 736f 7274  f.sort_by = sort
+0002ac30: 5f62 7920 2023 2074 7970 653a 2073 7472  _by  # type: str
+0002ac40: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+0002ac50: 6172 745f 7469 6d65 203d 2073 7461 7274  art_time = start
+0002ac60: 5f74 696d 6520 2023 2074 7970 653a 2073  _time  # type: s
+0002ac70: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+0002ac80: 7374 6174 7573 203d 2073 7461 7475 7320  status = status 
+0002ac90: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+0002aca0: 2020 2020 2073 656c 662e 7461 6773 5f73       self.tags_s
+0002acb0: 6872 696e 6b20 3d20 7461 6773 5f73 6872  hrink = tags_shr
+0002acc0: 696e 6b20 2023 2074 7970 653a 2073 7472  ink  # type: str
+0002acd0: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
+0002ace0: 726b 7370 6163 655f 6964 203d 2077 6f72  rkspace_id = wor
+0002acf0: 6b73 7061 6365 5f69 6420 2023 2074 7970  kspace_id  # typ
+0002ad00: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
+0002ad10: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+0002ad20: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+0002ad30: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0002ad40: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0002ad50: 203d 2073 7570 6572 284c 6973 744a 6f62   = super(ListJob
+0002ad60: 7353 6872 696e 6b52 6571 7565 7374 2c20  sShrinkRequest, 
+0002ad70: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+0002ad80: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0002ad90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002ada0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0002adb0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0002adc0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0002add0: 2020 2020 2069 6620 7365 6c66 2e62 7573       if self.bus
+0002ade0: 696e 6573 735f 7573 6572 5f69 6420 6973  iness_user_id is
+0002adf0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002ae00: 2020 2020 2020 2072 6573 756c 745b 2742         result['B
+0002ae10: 7573 696e 6573 7355 7365 7249 6427 5d20  usinessUserId'] 
+0002ae20: 3d20 7365 6c66 2e62 7573 696e 6573 735f  = self.business_
+0002ae30: 7573 6572 5f69 640a 2020 2020 2020 2020  user_id.        
+0002ae40: 6966 2073 656c 662e 6361 6c6c 6572 2069  if self.caller i
+0002ae50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002ae60: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002ae70: 4361 6c6c 6572 275d 203d 2073 656c 662e  Caller'] = self.
+0002ae80: 6361 6c6c 6572 0a20 2020 2020 2020 2069  caller.        i
+0002ae90: 6620 7365 6c66 2e64 6973 706c 6179 5f6e  f self.display_n
+0002aea0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
+0002aeb0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002aec0: 756c 745b 2744 6973 706c 6179 4e61 6d65  ult['DisplayName
+0002aed0: 275d 203d 2073 656c 662e 6469 7370 6c61  '] = self.displa
+0002aee0: 795f 6e61 6d65 0a20 2020 2020 2020 2069  y_name.        i
+0002aef0: 6620 7365 6c66 2e65 6e64 5f74 696d 6520  f self.end_time 
+0002af00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002af10: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002af20: 2745 6e64 5469 6d65 275d 203d 2073 656c  'EndTime'] = sel
+0002af30: 662e 656e 645f 7469 6d65 0a20 2020 2020  f.end_time.     
+0002af40: 2020 2069 6620 7365 6c66 2e66 726f 6d5f     if self.from_
+0002af50: 616c 6c5f 776f 726b 7370 6163 6573 2069  all_workspaces i
+0002af60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002af70: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002af80: 4672 6f6d 416c 6c57 6f72 6b73 7061 6365  FromAllWorkspace
+0002af90: 7327 5d20 3d20 7365 6c66 2e66 726f 6d5f  s'] = self.from_
+0002afa0: 616c 6c5f 776f 726b 7370 6163 6573 0a20  all_workspaces. 
+0002afb0: 2020 2020 2020 2069 6620 7365 6c66 2e6a         if self.j
+0002afc0: 6f62 5f69 6420 6973 206e 6f74 204e 6f6e  ob_id is not Non
+0002afd0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002afe0: 6573 756c 745b 274a 6f62 4964 275d 203d  esult['JobId'] =
+0002aff0: 2073 656c 662e 6a6f 625f 6964 0a20 2020   self.job_id.   
+0002b000: 2020 2020 2069 6620 7365 6c66 2e6a 6f62       if self.job
+0002b010: 5f74 7970 6520 6973 206e 6f74 204e 6f6e  _type is not Non
+0002b020: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002b030: 6573 756c 745b 274a 6f62 5479 7065 275d  esult['JobType']
+0002b040: 203d 2073 656c 662e 6a6f 625f 7479 7065   = self.job_type
+0002b050: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002b060: 2e6f 7264 6572 2069 7320 6e6f 7420 4e6f  .order is not No
+0002b070: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002b080: 7265 7375 6c74 5b27 4f72 6465 7227 5d20  result['Order'] 
+0002b090: 3d20 7365 6c66 2e6f 7264 6572 0a20 2020  = self.order.   
+0002b0a0: 2020 2020 2069 6620 7365 6c66 2e70 6167       if self.pag
+0002b0b0: 655f 6e75 6d62 6572 2069 7320 6e6f 7420  e_number is not 
+0002b0c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002b0d0: 2020 7265 7375 6c74 5b27 5061 6765 4e75    result['PageNu
+0002b0e0: 6d62 6572 275d 203d 2073 656c 662e 7061  mber'] = self.pa
+0002b0f0: 6765 5f6e 756d 6265 720a 2020 2020 2020  ge_number.      
+0002b100: 2020 6966 2073 656c 662e 7061 6765 5f73    if self.page_s
+0002b110: 697a 6520 6973 206e 6f74 204e 6f6e 653a  ize is not None:
+0002b120: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002b130: 756c 745b 2750 6167 6553 697a 6527 5d20  ult['PageSize'] 
+0002b140: 3d20 7365 6c66 2e70 6167 655f 7369 7a65  = self.page_size
+0002b150: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002b160: 2e70 6970 656c 696e 655f 6964 2069 7320  .pipeline_id is 
+0002b170: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002b180: 2020 2020 2020 7265 7375 6c74 5b27 5069        result['Pi
+0002b190: 7065 6c69 6e65 4964 275d 203d 2073 656c  pelineId'] = sel
+0002b1a0: 662e 7069 7065 6c69 6e65 5f69 640a 2020  f.pipeline_id.  
+0002b1b0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+0002b1c0: 736f 7572 6365 5f69 6420 6973 206e 6f74  source_id is not
+0002b1d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002b1e0: 2020 2072 6573 756c 745b 2752 6573 6f75     result['Resou
+0002b1f0: 7263 6549 6427 5d20 3d20 7365 6c66 2e72  rceId'] = self.r
+0002b200: 6573 6f75 7263 655f 6964 0a20 2020 2020  esource_id.     
+0002b210: 2020 2069 6620 7365 6c66 2e73 686f 775f     if self.show_
+0002b220: 6f77 6e20 6973 206e 6f74 204e 6f6e 653a  own is not None:
+0002b230: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002b240: 756c 745b 2753 686f 774f 776e 275d 203d  ult['ShowOwn'] =
+0002b250: 2073 656c 662e 7368 6f77 5f6f 776e 0a20   self.show_own. 
+0002b260: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0002b270: 6f72 745f 6279 2069 7320 6e6f 7420 4e6f  ort_by is not No
+0002b280: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002b290: 7265 7375 6c74 5b27 536f 7274 4279 275d  result['SortBy']
+0002b2a0: 203d 2073 656c 662e 736f 7274 5f62 790a   = self.sort_by.
+0002b2b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002b2c0: 7374 6172 745f 7469 6d65 2069 7320 6e6f  start_time is no
+0002b2d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b2e0: 2020 2020 7265 7375 6c74 5b27 5374 6172      result['Star
+0002b2f0: 7454 696d 6527 5d20 3d20 7365 6c66 2e73  tTime'] = self.s
+0002b300: 7461 7274 5f74 696d 650a 2020 2020 2020  tart_time.      
+0002b310: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+0002b320: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002b330: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002b340: 5b27 5374 6174 7573 275d 203d 2073 656c  ['Status'] = sel
+0002b350: 662e 7374 6174 7573 0a20 2020 2020 2020  f.status.       
+0002b360: 2069 6620 7365 6c66 2e74 6167 735f 7368   if self.tags_sh
+0002b370: 7269 6e6b 2069 7320 6e6f 7420 4e6f 6e65  rink is not None
+0002b380: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002b390: 7375 6c74 5b27 5461 6773 275d 203d 2073  sult['Tags'] = s
+0002b3a0: 656c 662e 7461 6773 5f73 6872 696e 6b0a  elf.tags_shrink.
+0002b3b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002b3c0: 776f 726b 7370 6163 655f 6964 2069 7320  workspace_id is 
+0002b3d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002b3e0: 2020 2020 2020 7265 7375 6c74 5b27 576f        result['Wo
+0002b3f0: 726b 7370 6163 6549 6427 5d20 3d20 7365  rkspaceId'] = se
+0002b400: 6c66 2e77 6f72 6b73 7061 6365 5f69 640a  lf.workspace_id.
+0002b410: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002b420: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0002b430: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0002b440: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0002b450: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0002b460: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002b470: 2742 7573 696e 6573 7355 7365 7249 6427  'BusinessUserId'
+0002b480: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002b490: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002b4a0: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
+0002b4b0: 203d 206d 2e67 6574 2827 4275 7369 6e65   = m.get('Busine
+0002b4c0: 7373 5573 6572 4964 2729 0a20 2020 2020  ssUserId').     
+0002b4d0: 2020 2069 6620 6d2e 6765 7428 2743 616c     if m.get('Cal
+0002b4e0: 6c65 7227 2920 6973 206e 6f74 204e 6f6e  ler') is not Non
+0002b4f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002b500: 656c 662e 6361 6c6c 6572 203d 206d 2e67  elf.caller = m.g
+0002b510: 6574 2827 4361 6c6c 6572 2729 0a20 2020  et('Caller').   
+0002b520: 2020 2020 2069 6620 6d2e 6765 7428 2744       if m.get('D
+0002b530: 6973 706c 6179 4e61 6d65 2729 2069 7320  isplayName') is 
+0002b540: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002b550: 2020 2020 2020 7365 6c66 2e64 6973 706c        self.displ
+0002b560: 6179 5f6e 616d 6520 3d20 6d2e 6765 7428  ay_name = m.get(
+0002b570: 2744 6973 706c 6179 4e61 6d65 2729 0a20  'DisplayName'). 
+0002b580: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002b590: 2745 6e64 5469 6d65 2729 2069 7320 6e6f  'EndTime') is no
+0002b5a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b5b0: 2020 2020 7365 6c66 2e65 6e64 5f74 696d      self.end_tim
+0002b5c0: 6520 3d20 6d2e 6765 7428 2745 6e64 5469  e = m.get('EndTi
+0002b5d0: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
+0002b5e0: 6d2e 6765 7428 2746 726f 6d41 6c6c 576f  m.get('FromAllWo
+0002b5f0: 726b 7370 6163 6573 2729 2069 7320 6e6f  rkspaces') is no
+0002b600: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b610: 2020 2020 7365 6c66 2e66 726f 6d5f 616c      self.from_al
+0002b620: 6c5f 776f 726b 7370 6163 6573 203d 206d  l_workspaces = m
+0002b630: 2e67 6574 2827 4672 6f6d 416c 6c57 6f72  .get('FromAllWor
+0002b640: 6b73 7061 6365 7327 290a 2020 2020 2020  kspaces').      
+0002b650: 2020 6966 206d 2e67 6574 2827 4a6f 6249    if m.get('JobI
+0002b660: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002b670: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002b680: 662e 6a6f 625f 6964 203d 206d 2e67 6574  f.job_id = m.get
+0002b690: 2827 4a6f 6249 6427 290a 2020 2020 2020  ('JobId').      
+0002b6a0: 2020 6966 206d 2e67 6574 2827 4a6f 6254    if m.get('JobT
+0002b6b0: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
+0002b6c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002b6d0: 656c 662e 6a6f 625f 7479 7065 203d 206d  elf.job_type = m
+0002b6e0: 2e67 6574 2827 4a6f 6254 7970 6527 290a  .get('JobType').
+0002b6f0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002b700: 2827 4f72 6465 7227 2920 6973 206e 6f74  ('Order') is not
+0002b710: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002b720: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
+0002b730: 6d2e 6765 7428 274f 7264 6572 2729 0a20  m.get('Order'). 
+0002b740: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002b750: 2750 6167 654e 756d 6265 7227 2920 6973  'PageNumber') is
+0002b760: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002b770: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
+0002b780: 5f6e 756d 6265 7220 3d20 6d2e 6765 7428  _number = m.get(
+0002b790: 2750 6167 654e 756d 6265 7227 290a 2020  'PageNumber').  
+0002b7a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002b7b0: 5061 6765 5369 7a65 2729 2069 7320 6e6f  PageSize') is no
+0002b7c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b7d0: 2020 2020 7365 6c66 2e70 6167 655f 7369      self.page_si
+0002b7e0: 7a65 203d 206d 2e67 6574 2827 5061 6765  ze = m.get('Page
+0002b7f0: 5369 7a65 2729 0a20 2020 2020 2020 2069  Size').        i
+0002b800: 6620 6d2e 6765 7428 2750 6970 656c 696e  f m.get('Pipelin
+0002b810: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+0002b820: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002b830: 656c 662e 7069 7065 6c69 6e65 5f69 6420  elf.pipeline_id 
+0002b840: 3d20 6d2e 6765 7428 2750 6970 656c 696e  = m.get('Pipelin
+0002b850: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
+0002b860: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+0002b870: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+0002b880: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002b890: 6c66 2e72 6573 6f75 7263 655f 6964 203d  lf.resource_id =
+0002b8a0: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+0002b8b0: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0002b8c0: 6d2e 6765 7428 2753 686f 774f 776e 2729  m.get('ShowOwn')
+0002b8d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002b8e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0002b8f0: 686f 775f 6f77 6e20 3d20 6d2e 6765 7428  how_own = m.get(
+0002b900: 2753 686f 774f 776e 2729 0a20 2020 2020  'ShowOwn').     
+0002b910: 2020 2069 6620 6d2e 6765 7428 2753 6f72     if m.get('Sor
+0002b920: 7442 7927 2920 6973 206e 6f74 204e 6f6e  tBy') is not Non
+0002b930: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002b940: 656c 662e 736f 7274 5f62 7920 3d20 6d2e  elf.sort_by = m.
+0002b950: 6765 7428 2753 6f72 7442 7927 290a 2020  get('SortBy').  
+0002b960: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002b970: 5374 6172 7454 696d 6527 2920 6973 206e  StartTime') is n
+0002b980: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002b990: 2020 2020 2073 656c 662e 7374 6172 745f       self.start_
+0002b9a0: 7469 6d65 203d 206d 2e67 6574 2827 5374  time = m.get('St
+0002b9b0: 6172 7454 696d 6527 290a 2020 2020 2020  artTime').      
+0002b9c0: 2020 6966 206d 2e67 6574 2827 5374 6174    if m.get('Stat
+0002b9d0: 7573 2729 2069 7320 6e6f 7420 4e6f 6e65  us') is not None
+0002b9e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002b9f0: 6c66 2e73 7461 7475 7320 3d20 6d2e 6765  lf.status = m.ge
+0002ba00: 7428 2753 7461 7475 7327 290a 2020 2020  t('Status').    
+0002ba10: 2020 2020 6966 206d 2e67 6574 2827 5461      if m.get('Ta
+0002ba20: 6773 2729 2069 7320 6e6f 7420 4e6f 6e65  gs') is not None
+0002ba30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002ba40: 6c66 2e74 6167 735f 7368 7269 6e6b 203d  lf.tags_shrink =
+0002ba50: 206d 2e67 6574 2827 5461 6773 2729 0a20   m.get('Tags'). 
+0002ba60: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002ba70: 2757 6f72 6b73 7061 6365 4964 2729 2069  'WorkspaceId') i
+0002ba80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002ba90: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+0002baa0: 6b73 7061 6365 5f69 6420 3d20 6d2e 6765  kspace_id = m.ge
+0002bab0: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
+0002bac0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002bad0: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
+0002bae0: 744a 6f62 7352 6573 706f 6e73 6542 6f64  tJobsResponseBod
+0002baf0: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+0002bb00: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0002bb10: 6c66 2c20 6a6f 6273 3d4e 6f6e 652c 2072  lf, jobs=None, r
+0002bb20: 6571 7565 7374 5f69 643d 4e6f 6e65 2c20  equest_id=None, 
+0002bb30: 746f 7461 6c5f 636f 756e 743d 4e6f 6e65  total_count=None
+0002bb40: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0002bb50: 6a6f 6273 203d 206a 6f62 7320 2023 2074  jobs = jobs  # t
+0002bb60: 7970 653a 206c 6973 745b 4a6f 6249 7465  ype: list[JobIte
+0002bb70: 6d5d 0a20 2020 2020 2020 2073 656c 662e  m].        self.
+0002bb80: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
+0002bb90: 7565 7374 5f69 6420 2023 2074 7970 653a  uest_id  # type:
+0002bba0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0002bbb0: 662e 746f 7461 6c5f 636f 756e 7420 3d20  f.total_count = 
+0002bbc0: 746f 7461 6c5f 636f 756e 7420 2023 2074  total_count  # t
+0002bbd0: 7970 653a 206c 6f6e 670a 0a20 2020 2064  ype: long..    d
+0002bbe0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0002bbf0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+0002bc00: 6c66 2e6a 6f62 733a 0a20 2020 2020 2020  lf.jobs:.       
+0002bc10: 2020 2020 2066 6f72 206b 2069 6e20 7365       for k in se
+0002bc20: 6c66 2e6a 6f62 733a 0a20 2020 2020 2020  lf.jobs:.       
+0002bc30: 2020 2020 2020 2020 2069 6620 6b3a 0a20           if k:. 
+0002bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002bc50: 2020 206b 2e76 616c 6964 6174 6528 290a     k.validate().
+0002bc60: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+0002bc70: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+0002bc80: 6d61 7020 3d20 7375 7065 7228 4c69 7374  map = super(List
+0002bc90: 4a6f 6273 5265 7370 6f6e 7365 426f 6479  JobsResponseBody
+0002bca0: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+0002bcb0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0002bcc0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002bcd0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002bce0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0002bcf0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0002bd00: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
+0002bd10: 6f62 7327 5d20 3d20 5b5d 0a20 2020 2020  obs'] = [].     
+0002bd20: 2020 2069 6620 7365 6c66 2e6a 6f62 7320     if self.jobs 
+0002bd30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002bd40: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
+0002bd50: 6e20 7365 6c66 2e6a 6f62 733a 0a20 2020  n self.jobs:.   
+0002bd60: 2020 2020 2020 2020 2020 2020 2072 6573               res
+0002bd70: 756c 745b 274a 6f62 7327 5d2e 6170 7065  ult['Jobs'].appe
+0002bd80: 6e64 286b 2e74 6f5f 6d61 7028 2920 6966  nd(k.to_map() if
+0002bd90: 206b 2065 6c73 6520 4e6f 6e65 290a 2020   k else None).  
+0002bda0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+0002bdb0: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
+0002bdc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002bdd0: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
+0002bde0: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
+0002bdf0: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
+0002be00: 6966 2073 656c 662e 746f 7461 6c5f 636f  if self.total_co
+0002be10: 756e 7420 6973 206e 6f74 204e 6f6e 653a  unt is not None:
+0002be20: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002be30: 756c 745b 2754 6f74 616c 436f 756e 7427  ult['TotalCount'
+0002be40: 5d20 3d20 7365 6c66 2e74 6f74 616c 5f63  ] = self.total_c
+0002be50: 6f75 6e74 0a20 2020 2020 2020 2072 6574  ount.        ret
+0002be60: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0002be70: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0002be80: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+0002be90: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+0002bea0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0002beb0: 2e6a 6f62 7320 3d20 5b5d 0a20 2020 2020  .jobs = [].     
+0002bec0: 2020 2069 6620 6d2e 6765 7428 274a 6f62     if m.get('Job
+0002bed0: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+0002bee0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0002bef0: 206b 2069 6e20 6d2e 6765 7428 274a 6f62   k in m.get('Job
+0002bf00: 7327 293a 0a20 2020 2020 2020 2020 2020  s'):.           
+0002bf10: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+0002bf20: 3d20 4a6f 6249 7465 6d28 290a 2020 2020  = JobItem().    
+0002bf30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002bf40: 2e6a 6f62 732e 6170 7065 6e64 2874 656d  .jobs.append(tem
+0002bf50: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+0002bf60: 286b 2929 0a20 2020 2020 2020 2069 6620  (k)).        if 
+0002bf70: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+0002bf80: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0002bf90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002bfa0: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
+0002bfb0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+0002bfc0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002bfd0: 7428 2754 6f74 616c 436f 756e 7427 2920  t('TotalCount') 
+0002bfe0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002bff0: 2020 2020 2020 2020 2073 656c 662e 746f           self.to
+0002c000: 7461 6c5f 636f 756e 7420 3d20 6d2e 6765  tal_count = m.ge
+0002c010: 7428 2754 6f74 616c 436f 756e 7427 290a  t('TotalCount').
+0002c020: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0002c030: 656c 660a 0a0a 636c 6173 7320 4c69 7374  elf...class List
+0002c040: 4a6f 6273 5265 7370 6f6e 7365 2854 6561  JobsResponse(Tea
+0002c050: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0002c060: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
+0002c070: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
+0002c080: 7475 735f 636f 6465 3d4e 6f6e 652c 2062  tus_code=None, b
+0002c090: 6f64 793d 4e6f 6e65 293a 0a20 2020 2020  ody=None):.     
+0002c0a0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+0002c0b0: 3d20 6865 6164 6572 7320 2023 2074 7970  = headers  # typ
+0002c0c0: 653a 2064 6963 745b 7374 722c 2073 7472  e: dict[str, str
+0002c0d0: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
+0002c0e0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+0002c0f0: 7475 735f 636f 6465 2020 2320 7479 7065  tus_code  # type
+0002c100: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
+0002c110: 6c66 2e62 6f64 7920 3d20 626f 6479 2020  lf.body = body  
+0002c120: 2320 7479 7065 3a20 4c69 7374 4a6f 6273  # type: ListJobs
+0002c130: 5265 7370 6f6e 7365 426f 6479 0a0a 2020  ResponseBody..  
+0002c140: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+0002c150: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+0002c160: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+0002c170: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
+0002c180: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
+0002c190: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+0002c1a0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+0002c1b0: 662e 7374 6174 7573 5f63 6f64 652c 2027  f.status_code, '
+0002c1c0: 7374 6174 7573 5f63 6f64 6527 290a 2020  status_code').  
+0002c1d0: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+0002c1e0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+0002c1f0: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
+0002c200: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002c210: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+0002c220: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+0002c230: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+0002c240: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+0002c250: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+0002c260: 6572 284c 6973 744a 6f62 7352 6573 706f  er(ListJobsRespo
+0002c270: 6e73 652c 2073 656c 6629 2e74 6f5f 6d61  nse, self).to_ma
+0002c280: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+0002c290: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+0002c2a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0002c2b0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+0002c2c0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+0002c2d0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0002c2e0: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+0002c2f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002c300: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+0002c310: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+0002c320: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+0002c330: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0002c340: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002c350: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002c360: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+0002c370: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0002c380: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002c390: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+0002c3a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002c3b0: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+0002c3c0: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+0002c3d0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+0002c3e0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0002c3f0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0002c400: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
+0002c410: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+0002c420: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002c430: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
+0002c440: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002c450: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+0002c460: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
+0002c470: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
+0002c480: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
+0002c490: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
+0002c4a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002c4b0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0002c4c0: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
+0002c4d0: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
+0002c4e0: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
+0002c4f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002c500: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+0002c510: 656c 203d 204c 6973 744a 6f62 7352 6573  el = ListJobsRes
+0002c520: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
+0002c530: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+0002c540: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
+0002c550: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
+0002c560: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+0002c570: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
+0002c580: 6973 7454 656e 736f 7262 6f61 7264 7352  istTensorboardsR
+0002c590: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+0002c5a0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0002c5b0: 5f5f 2873 656c 662c 2064 6973 706c 6179  __(self, display
+0002c5c0: 5f6e 616d 653d 4e6f 6e65 2c20 656e 645f  _name=None, end_
+0002c5d0: 7469 6d65 3d4e 6f6e 652c 206a 6f62 5f69  time=None, job_i
+0002c5e0: 643d 4e6f 6e65 2c20 6f72 6465 723d 4e6f  d=None, order=No
+0002c5f0: 6e65 2c20 7061 6765 5f6e 756d 6265 723d  ne, page_number=
+0002c600: 4e6f 6e65 2c20 7061 6765 5f73 697a 653d  None, page_size=
+0002c610: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0002c620: 2020 2020 2020 2073 6f72 745f 6279 3d4e         sort_by=N
+0002c630: 6f6e 652c 2073 6f75 7263 655f 6964 3d4e  one, source_id=N
+0002c640: 6f6e 652c 2073 6f75 7263 655f 7479 7065  one, source_type
+0002c650: 3d4e 6f6e 652c 2073 7461 7274 5f74 696d  =None, start_tim
+0002c660: 653d 4e6f 6e65 2c20 7374 6174 7573 3d4e  e=None, status=N
+0002c670: 6f6e 652c 2074 656e 736f 7262 6f61 7264  one, tensorboard
+0002c680: 5f69 643d 4e6f 6e65 2c0a 2020 2020 2020  _id=None,.      
+0002c690: 2020 2020 2020 2020 2020 2076 6572 626f             verbo
+0002c6a0: 7365 3d4e 6f6e 652c 2077 6f72 6b73 7061  se=None, workspa
+0002c6b0: 6365 5f69 643d 4e6f 6e65 293a 0a20 2020  ce_id=None):.   
+0002c6c0: 2020 2020 2073 656c 662e 6469 7370 6c61       self.displa
+0002c6d0: 795f 6e61 6d65 203d 2064 6973 706c 6179  y_name = display
+0002c6e0: 5f6e 616d 6520 2023 2074 7970 653a 2073  _name  # type: s
+0002c6f0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+0002c700: 656e 645f 7469 6d65 203d 2065 6e64 5f74  end_time = end_t
+0002c710: 696d 6520 2023 2074 7970 653a 2073 7472  ime  # type: str
+0002c720: 0a20 2020 2020 2020 2073 656c 662e 6a6f  .        self.jo
+0002c730: 625f 6964 203d 206a 6f62 5f69 6420 2023  b_id = job_id  #
+0002c740: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
+0002c750: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
+0002c760: 6f72 6465 7220 2023 2074 7970 653a 2073  order  # type: s
+0002c770: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+0002c780: 7061 6765 5f6e 756d 6265 7220 3d20 7061  page_number = pa
+0002c790: 6765 5f6e 756d 6265 7220 2023 2074 7970  ge_number  # typ
+0002c7a0: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
+0002c7b0: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
+0002c7c0: 7061 6765 5f73 697a 6520 2023 2074 7970  page_size  # typ
+0002c7d0: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
+0002c7e0: 656c 662e 736f 7274 5f62 7920 3d20 736f  elf.sort_by = so
+0002c7f0: 7274 5f62 7920 2023 2074 7970 653a 2073  rt_by  # type: s
+0002c800: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+0002c810: 736f 7572 6365 5f69 6420 3d20 736f 7572  source_id = sour
+0002c820: 6365 5f69 6420 2023 2074 7970 653a 2073  ce_id  # type: s
+0002c830: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+0002c840: 736f 7572 6365 5f74 7970 6520 3d20 736f  source_type = so
+0002c850: 7572 6365 5f74 7970 6520 2023 2074 7970  urce_type  # typ
+0002c860: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
+0002c870: 656c 662e 7374 6172 745f 7469 6d65 203d  elf.start_time =
+0002c880: 2073 7461 7274 5f74 696d 6520 2023 2074   start_time  # t
+0002c890: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+0002c8a0: 2073 656c 662e 7374 6174 7573 203d 2073   self.status = s
+0002c8b0: 7461 7475 7320 2023 2074 7970 653a 2073  tatus  # type: s
+0002c8c0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
+0002c8d0: 7465 6e73 6f72 626f 6172 645f 6964 203d  tensorboard_id =
+0002c8e0: 2074 656e 736f 7262 6f61 7264 5f69 6420   tensorboard_id 
+0002c8f0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+0002c900: 2020 2020 2073 656c 662e 7665 7262 6f73       self.verbos
+0002c910: 6520 3d20 7665 7262 6f73 6520 2023 2074  e = verbose  # t
+0002c920: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+0002c930: 2020 7365 6c66 2e77 6f72 6b73 7061 6365    self.workspace
+0002c940: 5f69 6420 3d20 776f 726b 7370 6163 655f  _id = workspace_
+0002c950: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+0002c960: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0002c970: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0002c980: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+0002c990: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0002c9a0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0002c9b0: 7228 4c69 7374 5465 6e73 6f72 626f 6172  r(ListTensorboar
+0002c9c0: 6473 5265 7175 6573 742c 2073 656c 6629  dsRequest, self)
+0002c9d0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0002c9e0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0002c9f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002ca00: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0002ca10: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0002ca20: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0002ca30: 6966 2073 656c 662e 6469 7370 6c61 795f  if self.display_
+0002ca40: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
+0002ca50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002ca60: 7375 6c74 5b27 4469 7370 6c61 794e 616d  sult['DisplayNam
+0002ca70: 6527 5d20 3d20 7365 6c66 2e64 6973 706c  e'] = self.displ
+0002ca80: 6179 5f6e 616d 650a 2020 2020 2020 2020  ay_name.        
+0002ca90: 6966 2073 656c 662e 656e 645f 7469 6d65  if self.end_time
+0002caa0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
 0002cab0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002cac0: 5b27 5465 6e73 6f72 626f 6172 6473 275d  ['Tensorboards']
-0002cad0: 2e61 7070 656e 6428 6b2e 746f 5f6d 6170  .append(k.to_map
-0002cae0: 2829 2069 6620 6b20 656c 7365 204e 6f6e  () if k else Non
-0002caf0: 6529 0a20 2020 2020 2020 2069 6620 7365  e).        if se
-0002cb00: 6c66 2e74 6f74 616c 5f63 6f75 6e74 2069  lf.total_count i
-0002cb10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002cb20: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002cb30: 546f 7461 6c43 6f75 6e74 275d 203d 2073  TotalCount'] = s
-0002cb40: 656c 662e 746f 7461 6c5f 636f 756e 740a  elf.total_count.
-0002cb50: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0002cb60: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-0002cb70: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
-0002cb80: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-0002cb90: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-0002cba0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002cbb0: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
-0002cbc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002cbd0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-0002cbe0: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
-0002cbf0: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
-0002cc00: 2020 2073 656c 662e 7465 6e73 6f72 626f     self.tensorbo
-0002cc10: 6172 6473 203d 205b 5d0a 2020 2020 2020  ards = [].      
-0002cc20: 2020 6966 206d 2e67 6574 2827 5465 6e73    if m.get('Tens
-0002cc30: 6f72 626f 6172 6473 2729 2069 7320 6e6f  orboards') is no
-0002cc40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002cc50: 2020 2020 666f 7220 6b20 696e 206d 2e67      for k in m.g
-0002cc60: 6574 2827 5465 6e73 6f72 626f 6172 6473  et('Tensorboards
-0002cc70: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-0002cc80: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-0002cc90: 2054 656e 736f 7262 6f61 7264 2829 0a20   Tensorboard(). 
-0002cca0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0002ccb0: 656c 662e 7465 6e73 6f72 626f 6172 6473  elf.tensorboards
-0002ccc0: 2e61 7070 656e 6428 7465 6d70 5f6d 6f64  .append(temp_mod
-0002ccd0: 656c 2e66 726f 6d5f 6d61 7028 6b29 290a  el.from_map(k)).
-0002cce0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002ccf0: 2827 546f 7461 6c43 6f75 6e74 2729 2069  ('TotalCount') i
-0002cd00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002cd10: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
-0002cd20: 616c 5f63 6f75 6e74 203d 206d 2e67 6574  al_count = m.get
-0002cd30: 2827 546f 7461 6c43 6f75 6e74 2729 0a20  ('TotalCount'). 
-0002cd40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0002cd50: 6c66 0a0a 0a63 6c61 7373 204c 6973 7454  lf...class ListT
-0002cd60: 656e 736f 7262 6f61 7264 7352 6573 706f  ensorboardsRespo
-0002cd70: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
-0002cd80: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0002cd90: 7365 6c66 2c20 6865 6164 6572 733d 4e6f  self, headers=No
-0002cda0: 6e65 2c20 7374 6174 7573 5f63 6f64 653d  ne, status_code=
-0002cdb0: 4e6f 6e65 2c20 626f 6479 3d4e 6f6e 6529  None, body=None)
-0002cdc0: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
-0002cdd0: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
-0002cde0: 2020 2320 7479 7065 3a20 6469 6374 5b73    # type: dict[s
-0002cdf0: 7472 2c20 7374 725d 0a20 2020 2020 2020  tr, str].       
-0002ce00: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0002ce10: 6520 3d20 7374 6174 7573 5f63 6f64 6520  e = status_code 
-0002ce20: 2023 2074 7970 653a 2069 6e74 0a20 2020   # type: int.   
-0002ce30: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-0002ce40: 2062 6f64 7920 2023 2074 7970 653a 204c   body  # type: L
-0002ce50: 6973 7454 656e 736f 7262 6f61 7264 7352  istTensorboardsR
-0002ce60: 6573 706f 6e73 6542 6f64 790a 0a20 2020  esponseBody..   
-0002ce70: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0002ce80: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-0002ce90: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-0002cea0: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
-0002ceb0: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
-0002cec0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-0002ced0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-0002cee0: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
-0002cef0: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
-0002cf00: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-0002cf10: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-0002cf20: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
-0002cf30: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0002cf40: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-0002cf50: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-0002cf60: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-0002cf70: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-0002cf80: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-0002cf90: 7228 4c69 7374 5465 6e73 6f72 626f 6172  r(ListTensorboar
-0002cfa0: 6473 5265 7370 6f6e 7365 2c20 7365 6c66  dsResponse, self
-0002cfb0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0002cfc0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0002cfd0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002cfe0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0002cff0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0002d000: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0002d010: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-0002d020: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002d030: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002d040: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-0002d050: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-0002d060: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-0002d070: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-0002d080: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002d090: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-0002d0a0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-0002d0b0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-0002d0c0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-0002d0d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002d0e0: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-0002d0f0: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-0002d100: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0002d110: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0002d120: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0002d130: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-0002d140: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-0002d150: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-0002d160: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-0002d170: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-0002d180: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002d190: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-0002d1a0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-0002d1b0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002d1c0: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-0002d1d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002d1e0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0002d1f0: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-0002d200: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-0002d210: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-0002d220: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-0002d230: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-0002d240: 656d 705f 6d6f 6465 6c20 3d20 4c69 7374  emp_model = List
-0002d250: 5465 6e73 6f72 626f 6172 6473 5265 7370  TensorboardsResp
-0002d260: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
-0002d270: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0002d280: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-0002d290: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
-0002d2a0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0002d2b0: 2073 656c 660a 0a0a 636c 6173 7320 5374   self...class St
-0002d2c0: 6172 7454 656e 736f 7262 6f61 7264 5265  artTensorboardRe
-0002d2d0: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-0002d2e0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0002d2f0: 5f28 7365 6c66 2c20 776f 726b 7370 6163  _(self, workspac
-0002d300: 655f 6964 3d4e 6f6e 6529 3a0a 2020 2020  e_id=None):.    
-0002d310: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
-0002d320: 6365 5f69 6420 3d20 776f 726b 7370 6163  ce_id = workspac
-0002d330: 655f 6964 2020 2320 7479 7065 3a20 7374  e_id  # type: st
-0002d340: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
-0002d350: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-0002d360: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-0002d370: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0002d380: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0002d390: 7065 7228 5374 6172 7454 656e 736f 7262  per(StartTensorb
-0002d3a0: 6f61 7264 5265 7175 6573 742c 2073 656c  oardRequest, sel
-0002d3b0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
-0002d3c0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0002d3d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002d3e0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0002d3f0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0002d400: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0002d410: 2020 6966 2073 656c 662e 776f 726b 7370    if self.worksp
-0002d420: 6163 655f 6964 2069 7320 6e6f 7420 4e6f  ace_id is not No
-0002d430: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002d440: 7265 7375 6c74 5b27 576f 726b 7370 6163  result['Workspac
-0002d450: 6549 6427 5d20 3d20 7365 6c66 2e77 6f72  eId'] = self.wor
-0002d460: 6b73 7061 6365 5f69 640a 2020 2020 2020  kspace_id.      
-0002d470: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0002d480: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0002d490: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-0002d4a0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-0002d4b0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-0002d4c0: 2069 6620 6d2e 6765 7428 2757 6f72 6b73   if m.get('Works
-0002d4d0: 7061 6365 4964 2729 2069 7320 6e6f 7420  paceId') is not 
-0002d4e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002d4f0: 2020 7365 6c66 2e77 6f72 6b73 7061 6365    self.workspace
-0002d500: 5f69 6420 3d20 6d2e 6765 7428 2757 6f72  _id = m.get('Wor
-0002d510: 6b73 7061 6365 4964 2729 0a20 2020 2020  kspaceId').     
-0002d520: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0002d530: 0a63 6c61 7373 2053 7461 7274 5465 6e73  .class StartTens
-0002d540: 6f72 626f 6172 6452 6573 706f 6e73 6542  orboardResponseB
-0002d550: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
-0002d560: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0002d570: 7365 6c66 2c20 7265 7175 6573 745f 6964  self, request_id
-0002d580: 3d4e 6f6e 652c 2074 656e 736f 7262 6f61  =None, tensorboa
-0002d590: 7264 5f69 643d 4e6f 6e65 293a 0a20 2020  rd_id=None):.   
-0002d5a0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-0002d5b0: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
-0002d5c0: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
-0002d5d0: 2020 2020 2020 2073 656c 662e 7465 6e73         self.tens
-0002d5e0: 6f72 626f 6172 645f 6964 203d 2074 656e  orboard_id = ten
-0002d5f0: 736f 7262 6f61 7264 5f69 6420 2023 2074  sorboard_id  # t
-0002d600: 7970 653a 2073 7472 0a0a 2020 2020 6465  ype: str..    de
-0002d610: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0002d620: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0002d630: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0002d640: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0002d650: 6170 203d 2073 7570 6572 2853 7461 7274  ap = super(Start
-0002d660: 5465 6e73 6f72 626f 6172 6452 6573 706f  TensorboardRespo
-0002d670: 6e73 6542 6f64 792c 2073 656c 6629 2e74  nseBody, self).t
-0002d680: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0002d690: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-0002d6a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002d6b0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-0002d6c0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-0002d6d0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0002d6e0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-0002d6f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002d700: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002d710: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
-0002d720: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
-0002d730: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002d740: 7465 6e73 6f72 626f 6172 645f 6964 2069  tensorboard_id i
-0002d750: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002d760: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002d770: 5465 6e73 6f72 626f 6172 6449 6427 5d20  TensorboardId'] 
-0002d780: 3d20 7365 6c66 2e74 656e 736f 7262 6f61  = self.tensorboa
-0002d790: 7264 5f69 640a 2020 2020 2020 2020 7265  rd_id.        re
-0002d7a0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-0002d7b0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-0002d7c0: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
-0002d7d0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-0002d7e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0002d7f0: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-0002d800: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002d810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002d820: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
-0002d830: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-0002d840: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002d850: 7428 2754 656e 736f 7262 6f61 7264 4964  t('TensorboardId
-0002d860: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002d870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002d880: 2e74 656e 736f 7262 6f61 7264 5f69 6420  .tensorboard_id 
-0002d890: 3d20 6d2e 6765 7428 2754 656e 736f 7262  = m.get('Tensorb
-0002d8a0: 6f61 7264 4964 2729 0a20 2020 2020 2020  oardId').       
-0002d8b0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0002d8c0: 6c61 7373 2053 7461 7274 5465 6e73 6f72  lass StartTensor
-0002d8d0: 626f 6172 6452 6573 706f 6e73 6528 5465  boardResponse(Te
-0002d8e0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-0002d8f0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-0002d900: 6865 6164 6572 733d 4e6f 6e65 2c20 7374  headers=None, st
-0002d910: 6174 7573 5f63 6f64 653d 4e6f 6e65 2c20  atus_code=None, 
-0002d920: 626f 6479 3d4e 6f6e 6529 3a0a 2020 2020  body=None):.    
-0002d930: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-0002d940: 203d 2068 6561 6465 7273 2020 2320 7479   = headers  # ty
-0002d950: 7065 3a20 6469 6374 5b73 7472 2c20 7374  pe: dict[str, st
-0002d960: 725d 0a20 2020 2020 2020 2073 656c 662e  r].        self.
-0002d970: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
-0002d980: 6174 7573 5f63 6f64 6520 2023 2074 7970  atus_code  # typ
-0002d990: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
-0002d9a0: 656c 662e 626f 6479 203d 2062 6f64 7920  elf.body = body 
-0002d9b0: 2023 2074 7970 653a 2053 7461 7274 5465   # type: StartTe
-0002d9c0: 6e73 6f72 626f 6172 6452 6573 706f 6e73  nsorboardRespons
-0002d9d0: 6542 6f64 790a 0a20 2020 2064 6566 2076  eBody..    def v
-0002d9e0: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0002d9f0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0002da00: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0002da10: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
-0002da20: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
-0002da30: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0002da40: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
-0002da50: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
-0002da60: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
-0002da70: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0002da80: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
-0002da90: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
-0002daa0: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-0002dab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002dac0: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-0002dad0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0002dae0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0002daf0: 6d61 7020 3d20 7375 7065 7228 5374 6172  map = super(Star
-0002db00: 7454 656e 736f 7262 6f61 7264 5265 7370  tTensorboardResp
-0002db10: 6f6e 7365 2c20 7365 6c66 292e 746f 5f6d  onse, self).to_m
-0002db20: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0002db30: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0002db40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002db50: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0002db60: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0002db70: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0002db80: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-0002db90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002dba0: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-0002dbb0: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-0002dbc0: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-0002dbd0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0002dbe0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002dbf0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002dc00: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-0002dc10: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0002dc20: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0002dc30: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-0002dc40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002dc50: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-0002dc60: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-0002dc70: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-0002dc80: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0002dc90: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0002dca0: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-0002dcb0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0002dcc0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0002dcd0: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-0002dce0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002dcf0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0002dd00: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-0002dd10: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-0002dd20: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-0002dd30: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-0002dd40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002dd50: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0002dd60: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-0002dd70: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-0002dd80: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-0002dd90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002dda0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-0002ddb0: 6465 6c20 3d20 5374 6172 7454 656e 736f  del = StartTenso
-0002ddc0: 7262 6f61 7264 5265 7370 6f6e 7365 426f  rboardResponseBo
-0002ddd0: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
-0002dde0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-0002ddf0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-0002de00: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-0002de10: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0002de20: 0a0a 636c 6173 7320 5374 6f70 4a6f 6252  ..class StopJobR
-0002de30: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-0002de40: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002de50: 5f69 6e69 745f 5f28 7365 6c66 2c20 6a6f  _init__(self, jo
-0002de60: 625f 6964 3d4e 6f6e 652c 2072 6571 7565  b_id=None, reque
-0002de70: 7374 5f69 643d 4e6f 6e65 293a 0a20 2020  st_id=None):.   
-0002de80: 2020 2020 2073 656c 662e 6a6f 625f 6964       self.job_id
-0002de90: 203d 206a 6f62 5f69 6420 2023 2074 7970   = job_id  # typ
-0002dea0: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-0002deb0: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-0002dec0: 2072 6571 7565 7374 5f69 6420 2023 2074   request_id  # t
-0002ded0: 7970 653a 2073 7472 0a0a 2020 2020 6465  ype: str..    de
-0002dee0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0002def0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0002df00: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0002df10: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0002df20: 6170 203d 2073 7570 6572 2853 746f 704a  ap = super(StopJ
-0002df30: 6f62 5265 7370 6f6e 7365 426f 6479 2c20  obResponseBody, 
-0002df40: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
-0002df50: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-0002df60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002df70: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-0002df80: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-0002df90: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-0002dfa0: 2020 2020 2069 6620 7365 6c66 2e6a 6f62       if self.job
-0002dfb0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-0002dfc0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002dfd0: 756c 745b 274a 6f62 4964 275d 203d 2073  ult['JobId'] = s
-0002dfe0: 656c 662e 6a6f 625f 6964 0a20 2020 2020  elf.job_id.     
-0002dff0: 2020 2069 6620 7365 6c66 2e72 6571 7565     if self.reque
-0002e000: 7374 5f69 6420 6973 206e 6f74 204e 6f6e  st_id is not Non
-0002e010: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002e020: 6573 756c 745b 2752 6571 7565 7374 4964  esult['RequestId
-0002e030: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
-0002e040: 745f 6964 0a20 2020 2020 2020 2072 6574  t_id.        ret
-0002e050: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0002e060: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0002e070: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-0002e080: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0002e090: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0002e0a0: 2e67 6574 2827 4a6f 6249 6427 2920 6973  .get('JobId') is
-0002e0b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002e0c0: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
-0002e0d0: 6964 203d 206d 2e67 6574 2827 4a6f 6249  id = m.get('JobI
-0002e0e0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-0002e0f0: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-0002e100: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002e110: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002e120: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
-0002e130: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
-0002e140: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0002e150: 656c 660a 0a0a 636c 6173 7320 5374 6f70  elf...class Stop
-0002e160: 4a6f 6252 6573 706f 6e73 6528 5465 614d  JobResponse(TeaM
-0002e170: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002e180: 5f69 6e69 745f 5f28 7365 6c66 2c20 6865  _init__(self, he
-0002e190: 6164 6572 733d 4e6f 6e65 2c20 7374 6174  aders=None, stat
-0002e1a0: 7573 5f63 6f64 653d 4e6f 6e65 2c20 626f  us_code=None, bo
-0002e1b0: 6479 3d4e 6f6e 6529 3a0a 2020 2020 2020  dy=None):.      
-0002e1c0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-0002e1d0: 2068 6561 6465 7273 2020 2320 7479 7065   headers  # type
-0002e1e0: 3a20 6469 6374 5b73 7472 2c20 7374 725d  : dict[str, str]
-0002e1f0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0002e200: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
-0002e210: 7573 5f63 6f64 6520 2023 2074 7970 653a  us_code  # type:
-0002e220: 2069 6e74 0a20 2020 2020 2020 2073 656c   int.        sel
-0002e230: 662e 626f 6479 203d 2062 6f64 7920 2023  f.body = body  #
-0002e240: 2074 7970 653a 2053 746f 704a 6f62 5265   type: StopJobRe
-0002e250: 7370 6f6e 7365 426f 6479 0a0a 2020 2020  sponseBody..    
-0002e260: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0002e270: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-0002e280: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0002e290: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
-0002e2a0: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
-0002e2b0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0002e2c0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0002e2d0: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
-0002e2e0: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
-0002e2f0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0002e300: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0002e310: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
-0002e320: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-0002e330: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-0002e340: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-0002e350: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-0002e360: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0002e370: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0002e380: 2853 746f 704a 6f62 5265 7370 6f6e 7365  (StopJobResponse
-0002e390: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
-0002e3a0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0002e3b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002e3c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002e3d0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0002e3e0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0002e3f0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-0002e400: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
-0002e410: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002e420: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
-0002e430: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
-0002e440: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002e450: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
-0002e460: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002e470: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
-0002e480: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
-0002e490: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
-0002e4a0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-0002e4b0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
-0002e4c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002e4d0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
-0002e4e0: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
-0002e4f0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0002e500: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-0002e510: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
-0002e520: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-0002e530: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-0002e540: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002e550: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
-0002e560: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002e570: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-0002e580: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
-0002e590: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-0002e5a0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-0002e5b0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002e5c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002e5d0: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
-0002e5e0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
-0002e5f0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0002e600: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
-0002e610: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002e620: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-0002e630: 3d20 5374 6f70 4a6f 6252 6573 706f 6e73  = StopJobRespons
-0002e640: 6542 6f64 7928 290a 2020 2020 2020 2020  eBody().        
-0002e650: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-0002e660: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-0002e670: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
-0002e680: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0002e690: 6c66 0a0a 0a63 6c61 7373 2053 746f 7054  lf...class StopT
-0002e6a0: 656e 736f 7262 6f61 7264 5265 7175 6573  ensorboardReques
-0002e6b0: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
-0002e6c0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-0002e6d0: 6c66 2c20 776f 726b 7370 6163 655f 6964  lf, workspace_id
-0002e6e0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0002e6f0: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
-0002e700: 6420 3d20 776f 726b 7370 6163 655f 6964  d = workspace_id
-0002e710: 2020 2320 7479 7065 3a20 7374 720a 0a20    # type: str.. 
-0002e720: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0002e730: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0002e740: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-0002e750: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0002e760: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0002e770: 5374 6f70 5465 6e73 6f72 626f 6172 6452  StopTensorboardR
-0002e780: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
-0002e790: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0002e7a0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0002e7b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002e7c0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0002e7d0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0002e7e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0002e7f0: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
-0002e800: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-0002e810: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002e820: 745b 2757 6f72 6b73 7061 6365 4964 275d  t['WorkspaceId']
-0002e830: 203d 2073 656c 662e 776f 726b 7370 6163   = self.workspac
-0002e840: 655f 6964 0a20 2020 2020 2020 2072 6574  e_id.        ret
-0002e850: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0002e860: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0002e870: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-0002e880: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0002e890: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0002e8a0: 2e67 6574 2827 576f 726b 7370 6163 6549  .get('WorkspaceI
-0002e8b0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-0002e8c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002e8d0: 662e 776f 726b 7370 6163 655f 6964 203d  f.workspace_id =
-0002e8e0: 206d 2e67 6574 2827 576f 726b 7370 6163   m.get('Workspac
-0002e8f0: 6549 6427 290a 2020 2020 2020 2020 7265  eId').        re
-0002e900: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-0002e910: 7320 5374 6f70 5465 6e73 6f72 626f 6172  s StopTensorboar
-0002e920: 6452 6573 706f 6e73 6542 6f64 7928 5465  dResponseBody(Te
-0002e930: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-0002e940: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-0002e950: 7265 7175 6573 745f 6964 3d4e 6f6e 652c  request_id=None,
-0002e960: 2074 656e 736f 7262 6f61 7264 5f69 643d   tensorboard_id=
-0002e970: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-0002e980: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-0002e990: 2072 6571 7565 7374 5f69 6420 2023 2074   request_id  # t
-0002e9a0: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
-0002e9b0: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
-0002e9c0: 645f 6964 203d 2074 656e 736f 7262 6f61  d_id = tensorboa
-0002e9d0: 7264 5f69 6420 2023 2074 7970 653a 2073  rd_id  # type: s
-0002e9e0: 7472 0a0a 2020 2020 6465 6620 7661 6c69  tr..    def vali
-0002e9f0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-0002ea00: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-0002ea10: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0002ea20: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0002ea30: 7570 6572 2853 746f 7054 656e 736f 7262  uper(StopTensorb
-0002ea40: 6f61 7264 5265 7370 6f6e 7365 426f 6479  oardResponseBody
-0002ea50: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
-0002ea60: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0002ea70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002ea80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002ea90: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0002eaa0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0002eab0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0002eac0: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
-0002ead0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002eae0: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
-0002eaf0: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
-0002eb00: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
-0002eb10: 2069 6620 7365 6c66 2e74 656e 736f 7262   if self.tensorb
-0002eb20: 6f61 7264 5f69 6420 6973 206e 6f74 204e  oard_id is not N
-0002eb30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002eb40: 2072 6573 756c 745b 2754 656e 736f 7262   result['Tensorb
-0002eb50: 6f61 7264 4964 275d 203d 2073 656c 662e  oardId'] = self.
-0002eb60: 7465 6e73 6f72 626f 6172 645f 6964 0a20  tensorboard_id. 
-0002eb70: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002eb80: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0002eb90: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-0002eba0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0002ebb0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0002ebc0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002ebd0: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
-0002ebe0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002ebf0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-0002ec00: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
-0002ec10: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
-0002ec20: 2020 6966 206d 2e67 6574 2827 5465 6e73    if m.get('Tens
-0002ec30: 6f72 626f 6172 6449 6427 2920 6973 206e  orboardId') is n
-0002ec40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002ec50: 2020 2020 2073 656c 662e 7465 6e73 6f72       self.tensor
-0002ec60: 626f 6172 645f 6964 203d 206d 2e67 6574  board_id = m.get
-0002ec70: 2827 5465 6e73 6f72 626f 6172 6449 6427  ('TensorboardId'
-0002ec80: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0002ec90: 2073 656c 660a 0a0a 636c 6173 7320 5374   self...class St
-0002eca0: 6f70 5465 6e73 6f72 626f 6172 6452 6573  opTensorboardRes
-0002ecb0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-0002ecc0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0002ecd0: 5f28 7365 6c66 2c20 6865 6164 6572 733d  _(self, headers=
-0002ece0: 4e6f 6e65 2c20 7374 6174 7573 5f63 6f64  None, status_cod
-0002ecf0: 653d 4e6f 6e65 2c20 626f 6479 3d4e 6f6e  e=None, body=Non
-0002ed00: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-0002ed10: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
-0002ed20: 7273 2020 2320 7479 7065 3a20 6469 6374  rs  # type: dict
-0002ed30: 5b73 7472 2c20 7374 725d 0a20 2020 2020  [str, str].     
-0002ed40: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-0002ed50: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-0002ed60: 6520 2023 2074 7970 653a 2069 6e74 0a20  e  # type: int. 
-0002ed70: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0002ed80: 203d 2062 6f64 7920 2023 2074 7970 653a   = body  # type:
-0002ed90: 2053 746f 7054 656e 736f 7262 6f61 7264   StopTensorboard
-0002eda0: 5265 7370 6f6e 7365 426f 6479 0a0a 2020  ResponseBody..  
-0002edb0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0002edc0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-0002edd0: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-0002ede0: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
-0002edf0: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
-0002ee00: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0002ee10: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-0002ee20: 662e 7374 6174 7573 5f63 6f64 652c 2027  f.status_code, '
-0002ee30: 7374 6174 7573 5f63 6f64 6527 290a 2020  status_code').  
-0002ee40: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0002ee50: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-0002ee60: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
-0002ee70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002ee80: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-0002ee90: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-0002eea0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-0002eeb0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0002eec0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0002eed0: 6572 2853 746f 7054 656e 736f 7262 6f61  er(StopTensorboa
-0002eee0: 7264 5265 7370 6f6e 7365 2c20 7365 6c66  rdResponse, self
-0002eef0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0002ef00: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0002ef10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002ef20: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0002ef30: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0002ef40: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0002ef50: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
-0002ef60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002ef70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002ef80: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
-0002ef90: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
-0002efa0: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
-0002efb0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
-0002efc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002efd0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
-0002efe0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
-0002eff0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
-0002f000: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
-0002f010: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002f020: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
-0002f030: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
-0002f040: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0002f050: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0002f060: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0002f070: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-0002f080: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-0002f090: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-0002f0a0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-0002f0b0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-0002f0c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002f0d0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-0002f0e0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-0002f0f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002f100: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-0002f110: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002f120: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0002f130: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-0002f140: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-0002f150: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-0002f160: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-0002f170: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-0002f180: 656d 705f 6d6f 6465 6c20 3d20 5374 6f70  emp_model = Stop
-0002f190: 5465 6e73 6f72 626f 6172 6452 6573 706f  TensorboardRespo
-0002f1a0: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
-0002f1b0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-0002f1c0: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
-0002f1d0: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
-0002f1e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002f1f0: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
-0002f200: 6174 654a 6f62 5265 7175 6573 7428 5465  ateJobRequest(Te
-0002f210: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-0002f220: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-0002f230: 7072 696f 7269 7479 3d4e 6f6e 6529 3a0a  priority=None):.
-0002f240: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
-0002f250: 6f72 6974 7920 3d20 7072 696f 7269 7479  ority = priority
-0002f260: 2020 2320 7479 7065 3a20 696e 740a 0a20    # type: int.. 
-0002f270: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0002f280: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0002f290: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
-0002f2a0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0002f2b0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0002f2c0: 5570 6461 7465 4a6f 6252 6571 7565 7374  UpdateJobRequest
-0002f2d0: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
-0002f2e0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0002f2f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002f300: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002f310: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0002f320: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0002f330: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0002f340: 7269 6f72 6974 7920 6973 206e 6f74 204e  riority is not N
-0002f350: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002f360: 2072 6573 756c 745b 2750 7269 6f72 6974   result['Priorit
-0002f370: 7927 5d20 3d20 7365 6c66 2e70 7269 6f72  y'] = self.prior
-0002f380: 6974 790a 2020 2020 2020 2020 7265 7475  ity.        retu
-0002f390: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0002f3a0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0002f3b0: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-0002f3c0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0002f3d0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0002f3e0: 6765 7428 2750 7269 6f72 6974 7927 2920  get('Priority') 
-0002f3f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002f400: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0002f410: 696f 7269 7479 203d 206d 2e67 6574 2827  iority = m.get('
-0002f420: 5072 696f 7269 7479 2729 0a20 2020 2020  Priority').     
-0002f430: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0002f440: 0a63 6c61 7373 2055 7064 6174 654a 6f62  .class UpdateJob
-0002f450: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
-0002f460: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0002f470: 5f5f 696e 6974 5f5f 2873 656c 662c 206a  __init__(self, j
-0002f480: 6f62 5f69 643d 4e6f 6e65 2c20 7265 7175  ob_id=None, requ
-0002f490: 6573 745f 6964 3d4e 6f6e 6529 3a0a 2020  est_id=None):.  
-0002f4a0: 2020 2020 2020 7365 6c66 2e6a 6f62 5f69        self.job_i
-0002f4b0: 6420 3d20 6a6f 625f 6964 2020 2320 7479  d = job_id  # ty
-0002f4c0: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-0002f4d0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-0002f4e0: 3d20 7265 7175 6573 745f 6964 2020 2320  = request_id  # 
-0002f4f0: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
-0002f500: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0002f510: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0002f520: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0002f530: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0002f540: 6d61 7020 3d20 7375 7065 7228 5570 6461  map = super(Upda
-0002f550: 7465 4a6f 6252 6573 706f 6e73 6542 6f64  teJobResponseBod
-0002f560: 792c 2073 656c 6629 2e74 6f5f 6d61 7028  y, self).to_map(
-0002f570: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-0002f580: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-0002f590: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0002f5a0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-0002f5b0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-0002f5c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002f5d0: 6a6f 625f 6964 2069 7320 6e6f 7420 4e6f  job_id is not No
-0002f5e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002f5f0: 7265 7375 6c74 5b27 4a6f 6249 6427 5d20  result['JobId'] 
-0002f600: 3d20 7365 6c66 2e6a 6f62 5f69 640a 2020  = self.job_id.  
-0002f610: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-0002f620: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
-0002f630: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002f640: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
-0002f650: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
-0002f660: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
-0002f670: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0002f680: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0002f690: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
-0002f6a0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-0002f6b0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0002f6c0: 6620 6d2e 6765 7428 274a 6f62 4964 2729  f m.get('JobId')
-0002f6d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002f6e0: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
-0002f6f0: 6f62 5f69 6420 3d20 6d2e 6765 7428 274a  ob_id = m.get('J
-0002f700: 6f62 4964 2729 0a20 2020 2020 2020 2069  obId').        i
-0002f710: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
-0002f720: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-0002f730: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002f740: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-0002f750: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-0002f760: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0002f770: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
-0002f780: 7064 6174 654a 6f62 5265 7370 6f6e 7365  pdateJobResponse
-0002f790: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-0002f7a0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0002f7b0: 662c 2068 6561 6465 7273 3d4e 6f6e 652c  f, headers=None,
-0002f7c0: 2073 7461 7475 735f 636f 6465 3d4e 6f6e   status_code=Non
-0002f7d0: 652c 2062 6f64 793d 4e6f 6e65 293a 0a20  e, body=None):. 
-0002f7e0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0002f7f0: 6572 7320 3d20 6865 6164 6572 7320 2023  ers = headers  #
-0002f800: 2074 7970 653a 2064 6963 745b 7374 722c   type: dict[str,
-0002f810: 2073 7472 5d0a 2020 2020 2020 2020 7365   str].        se
-0002f820: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-0002f830: 2073 7461 7475 735f 636f 6465 2020 2320   status_code  # 
-0002f840: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
-0002f850: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-0002f860: 6479 2020 2320 7479 7065 3a20 5570 6461  dy  # type: Upda
-0002f870: 7465 4a6f 6252 6573 706f 6e73 6542 6f64  teJobResponseBod
-0002f880: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-0002f890: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-0002f8a0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-0002f8b0: 5f72 6571 7569 7265 6428 7365 6c66 2e68  _required(self.h
-0002f8c0: 6561 6465 7273 2c20 2768 6561 6465 7273  eaders, 'headers
-0002f8d0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-0002f8e0: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-0002f8f0: 6428 7365 6c66 2e73 7461 7475 735f 636f  d(self.status_co
-0002f900: 6465 2c20 2773 7461 7475 735f 636f 6465  de, 'status_code
-0002f910: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-0002f920: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-0002f930: 6428 7365 6c66 2e62 6f64 792c 2027 626f  d(self.body, 'bo
-0002f940: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
-0002f950: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-0002f960: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0002f970: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-0002f980: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-0002f990: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-0002f9a0: 3d20 7375 7065 7228 5570 6461 7465 4a6f  = super(UpdateJo
-0002f9b0: 6252 6573 706f 6e73 652c 2073 656c 6629  bResponse, self)
-0002f9c0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0002f9d0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0002f9e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002f9f0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0002fa00: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0002fa10: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002fa20: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-0002fa30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002fa40: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002fa50: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-0002fa60: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-0002fa70: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-0002fa80: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-0002fa90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002faa0: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-0002fab0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-0002fac0: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-0002fad0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-0002fae0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002faf0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-0002fb00: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-0002fb10: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0002fb20: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0002fb30: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0002fb40: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-0002fb50: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0002fb60: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002fb70: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
-0002fb80: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-0002fb90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002fba0: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
-0002fbb0: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
-0002fbc0: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
-0002fbd0: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
-0002fbe0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002fbf0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-0002fc00: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
-0002fc10: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
-0002fc20: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-0002fc30: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-0002fc40: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-0002fc50: 6d70 5f6d 6f64 656c 203d 2055 7064 6174  mp_model = Updat
-0002fc60: 654a 6f62 5265 7370 6f6e 7365 426f 6479  eJobResponseBody
-0002fc70: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-0002fc80: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-0002fc90: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-0002fca0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-0002fcb0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0002fcc0: 636c 6173 7320 5570 6461 7465 5465 6e73  class UpdateTens
-0002fcd0: 6f72 626f 6172 6452 6571 7565 7374 2854  orboardRequest(T
-0002fce0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-0002fcf0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0002fd00: 206d 6178 5f72 756e 6e69 6e67 5f74 696d   max_running_tim
-0002fd10: 655f 6d69 6e75 7465 733d 4e6f 6e65 2c20  e_minutes=None, 
-0002fd20: 776f 726b 7370 6163 655f 6964 3d4e 6f6e  workspace_id=Non
-0002fd30: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-0002fd40: 2e6d 6178 5f72 756e 6e69 6e67 5f74 696d  .max_running_tim
-0002fd50: 655f 6d69 6e75 7465 7320 3d20 6d61 785f  e_minutes = max_
-0002fd60: 7275 6e6e 696e 675f 7469 6d65 5f6d 696e  running_time_min
-0002fd70: 7574 6573 2020 2320 7479 7065 3a20 6c6f  utes  # type: lo
-0002fd80: 6e67 0a20 2020 2020 2020 2073 656c 662e  ng.        self.
-0002fd90: 776f 726b 7370 6163 655f 6964 203d 2077  workspace_id = w
-0002fda0: 6f72 6b73 7061 6365 5f69 6420 2023 2074  orkspace_id  # t
-0002fdb0: 7970 653a 2073 7472 0a0a 2020 2020 6465  ype: str..    de
-0002fdc0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0002fdd0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0002fde0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0002fdf0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0002fe00: 6170 203d 2073 7570 6572 2855 7064 6174  ap = super(Updat
-0002fe10: 6554 656e 736f 7262 6f61 7264 5265 7175  eTensorboardRequ
-0002fe20: 6573 742c 2073 656c 6629 2e74 6f5f 6d61  est, self).to_ma
-0002fe30: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0002fe40: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0002fe50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0002fe60: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0002fe70: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0002fe80: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0002fe90: 662e 6d61 785f 7275 6e6e 696e 675f 7469  f.max_running_ti
-0002fea0: 6d65 5f6d 696e 7574 6573 2069 7320 6e6f  me_minutes is no
-0002feb0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002fec0: 2020 2020 7265 7375 6c74 5b27 4d61 7852      result['MaxR
-0002fed0: 756e 6e69 6e67 5469 6d65 4d69 6e75 7465  unningTimeMinute
-0002fee0: 7327 5d20 3d20 7365 6c66 2e6d 6178 5f72  s'] = self.max_r
-0002fef0: 756e 6e69 6e67 5f74 696d 655f 6d69 6e75  unning_time_minu
-0002ff00: 7465 730a 2020 2020 2020 2020 6966 2073  tes.        if s
-0002ff10: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-0002ff20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002ff30: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002ff40: 5b27 576f 726b 7370 6163 6549 6427 5d20  ['WorkspaceId'] 
-0002ff50: 3d20 7365 6c66 2e77 6f72 6b73 7061 6365  = self.workspace
-0002ff60: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-0002ff70: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0002ff80: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0002ff90: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-0002ffa0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0002ffb0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0002ffc0: 6765 7428 274d 6178 5275 6e6e 696e 6754  get('MaxRunningT
-0002ffd0: 696d 654d 696e 7574 6573 2729 2069 7320  imeMinutes') is 
-0002ffe0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002fff0: 2020 2020 2020 7365 6c66 2e6d 6178 5f72        self.max_r
-00030000: 756e 6e69 6e67 5f74 696d 655f 6d69 6e75  unning_time_minu
-00030010: 7465 7320 3d20 6d2e 6765 7428 274d 6178  tes = m.get('Max
-00030020: 5275 6e6e 696e 6754 696d 654d 696e 7574  RunningTimeMinut
-00030030: 6573 2729 0a20 2020 2020 2020 2069 6620  es').        if 
-00030040: 6d2e 6765 7428 2757 6f72 6b73 7061 6365  m.get('Workspace
-00030050: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-00030060: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00030070: 6c66 2e77 6f72 6b73 7061 6365 5f69 6420  lf.workspace_id 
-00030080: 3d20 6d2e 6765 7428 2757 6f72 6b73 7061  = m.get('Workspa
-00030090: 6365 4964 2729 0a20 2020 2020 2020 2072  ceId').        r
-000300a0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-000300b0: 7373 2055 7064 6174 6554 656e 736f 7262  ss UpdateTensorb
-000300c0: 6f61 7264 5265 7370 6f6e 7365 426f 6479  oardResponseBody
-000300d0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-000300e0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-000300f0: 662c 2072 6571 7565 7374 5f69 643d 4e6f  f, request_id=No
-00030100: 6e65 2c20 7465 6e73 6f72 626f 6172 645f  ne, tensorboard_
-00030110: 6964 3d4e 6f6e 6529 3a0a 2020 2020 2020  id=None):.      
-00030120: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
-00030130: 6420 3d20 7265 7175 6573 745f 6964 2020  d = request_id  
-00030140: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00030150: 2020 2020 7365 6c66 2e74 656e 736f 7262      self.tensorb
-00030160: 6f61 7264 5f69 6420 3d20 7465 6e73 6f72  oard_id = tensor
-00030170: 626f 6172 645f 6964 2020 2320 7479 7065  board_id  # type
-00030180: 3a20 7374 720a 0a20 2020 2064 6566 2076  : str..    def v
-00030190: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-000301a0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-000301b0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-000301c0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-000301d0: 3d20 7375 7065 7228 5570 6461 7465 5465  = super(UpdateTe
-000301e0: 6e73 6f72 626f 6172 6452 6573 706f 6e73  nsorboardRespons
-000301f0: 6542 6f64 792c 2073 656c 6629 2e74 6f5f  eBody, self).to_
-00030200: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-00030210: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-00030220: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00030230: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-00030240: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-00030250: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00030260: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
-00030270: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00030280: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00030290: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
-000302a0: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
-000302b0: 2020 2020 2020 6966 2073 656c 662e 7465        if self.te
-000302c0: 6e73 6f72 626f 6172 645f 6964 2069 7320  nsorboard_id is 
-000302d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000302e0: 2020 2020 2020 7265 7375 6c74 5b27 5465        result['Te
-000302f0: 6e73 6f72 626f 6172 6449 6427 5d20 3d20  nsorboardId'] = 
-00030300: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
-00030310: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-00030320: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00030330: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00030340: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-00030350: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-00030360: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-00030370: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-00030380: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00030390: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000303a0: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
-000303b0: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
-000303c0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000303d0: 2754 656e 736f 7262 6f61 7264 4964 2729  'TensorboardId')
-000303e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000303f0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00030400: 656e 736f 7262 6f61 7264 5f69 6420 3d20  ensorboard_id = 
-00030410: 6d2e 6765 7428 2754 656e 736f 7262 6f61  m.get('Tensorboa
-00030420: 7264 4964 2729 0a20 2020 2020 2020 2072  rdId').        r
-00030430: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-00030440: 7373 2055 7064 6174 6554 656e 736f 7262  ss UpdateTensorb
-00030450: 6f61 7264 5265 7370 6f6e 7365 2854 6561  oardResponse(Tea
-00030460: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00030470: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
-00030480: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
-00030490: 7475 735f 636f 6465 3d4e 6f6e 652c 2062  tus_code=None, b
-000304a0: 6f64 793d 4e6f 6e65 293a 0a20 2020 2020  ody=None):.     
-000304b0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-000304c0: 3d20 6865 6164 6572 7320 2023 2074 7970  = headers  # typ
-000304d0: 653a 2064 6963 745b 7374 722c 2073 7472  e: dict[str, str
-000304e0: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
-000304f0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-00030500: 7475 735f 636f 6465 2020 2320 7479 7065  tus_code  # type
-00030510: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
-00030520: 6c66 2e62 6f64 7920 3d20 626f 6479 2020  lf.body = body  
-00030530: 2320 7479 7065 3a20 5570 6461 7465 5465  # type: UpdateTe
-00030540: 6e73 6f72 626f 6172 6452 6573 706f 6e73  nsorboardRespons
-00030550: 6542 6f64 790a 0a20 2020 2064 6566 2076  eBody..    def v
-00030560: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-00030570: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-00030580: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-00030590: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
-000305a0: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
-000305b0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-000305c0: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
-000305d0: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
-000305e0: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
-000305f0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-00030600: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
-00030610: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
-00030620: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-00030630: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00030640: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-00030650: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00030660: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00030670: 6d61 7020 3d20 7375 7065 7228 5570 6461  map = super(Upda
-00030680: 7465 5465 6e73 6f72 626f 6172 6452 6573  teTensorboardRes
-00030690: 706f 6e73 652c 2073 656c 6629 2e74 6f5f  ponse, self).to_
-000306a0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-000306b0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-000306c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000306d0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-000306e0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-000306f0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-00030700: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
-00030710: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00030720: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
-00030730: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
-00030740: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
-00030750: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00030760: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00030770: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00030780: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
-00030790: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
-000307a0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
-000307b0: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
-000307c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000307d0: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
-000307e0: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
-000307f0: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
-00030800: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00030810: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-00030820: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-00030830: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-00030840: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-00030850: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
-00030860: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00030870: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-00030880: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
-00030890: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
-000308a0: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
-000308b0: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
-000308c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000308d0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-000308e0: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
-000308f0: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
-00030900: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
-00030910: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00030920: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-00030930: 6f64 656c 203d 2055 7064 6174 6554 656e  odel = UpdateTen
-00030940: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
-00030950: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
-00030960: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-00030970: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-00030980: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-00030990: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000309a0: 660a 0a0a                                f...
+0002cac0: 5b27 456e 6454 696d 6527 5d20 3d20 7365  ['EndTime'] = se
+0002cad0: 6c66 2e65 6e64 5f74 696d 650a 2020 2020  lf.end_time.    
+0002cae0: 2020 2020 6966 2073 656c 662e 6a6f 625f      if self.job_
+0002caf0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0002cb00: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002cb10: 6c74 5b27 4a6f 6249 6427 5d20 3d20 7365  lt['JobId'] = se
+0002cb20: 6c66 2e6a 6f62 5f69 640a 2020 2020 2020  lf.job_id.      
+0002cb30: 2020 6966 2073 656c 662e 6f72 6465 7220    if self.order 
+0002cb40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002cb50: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002cb60: 274f 7264 6572 275d 203d 2073 656c 662e  'Order'] = self.
+0002cb70: 6f72 6465 720a 2020 2020 2020 2020 6966  order.        if
+0002cb80: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
+0002cb90: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+0002cba0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002cbb0: 745b 2750 6167 654e 756d 6265 7227 5d20  t['PageNumber'] 
+0002cbc0: 3d20 7365 6c66 2e70 6167 655f 6e75 6d62  = self.page_numb
+0002cbd0: 6572 0a20 2020 2020 2020 2069 6620 7365  er.        if se
+0002cbe0: 6c66 2e70 6167 655f 7369 7a65 2069 7320  lf.page_size is 
+0002cbf0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002cc00: 2020 2020 2020 7265 7375 6c74 5b27 5061        result['Pa
+0002cc10: 6765 5369 7a65 275d 203d 2073 656c 662e  geSize'] = self.
+0002cc20: 7061 6765 5f73 697a 650a 2020 2020 2020  page_size.      
+0002cc30: 2020 6966 2073 656c 662e 736f 7274 5f62    if self.sort_b
+0002cc40: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0002cc50: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002cc60: 745b 2753 6f72 7442 7927 5d20 3d20 7365  t['SortBy'] = se
+0002cc70: 6c66 2e73 6f72 745f 6279 0a20 2020 2020  lf.sort_by.     
+0002cc80: 2020 2069 6620 7365 6c66 2e73 6f75 7263     if self.sourc
+0002cc90: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+0002cca0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002ccb0: 7375 6c74 5b27 536f 7572 6365 4964 275d  sult['SourceId']
+0002ccc0: 203d 2073 656c 662e 736f 7572 6365 5f69   = self.source_i
+0002ccd0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+0002cce0: 662e 736f 7572 6365 5f74 7970 6520 6973  f.source_type is
+0002ccf0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002cd00: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
+0002cd10: 6f75 7263 6554 7970 6527 5d20 3d20 7365  ourceType'] = se
+0002cd20: 6c66 2e73 6f75 7263 655f 7479 7065 0a20  lf.source_type. 
+0002cd30: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0002cd40: 7461 7274 5f74 696d 6520 6973 206e 6f74  tart_time is not
+0002cd50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002cd60: 2020 2072 6573 756c 745b 2753 7461 7274     result['Start
+0002cd70: 5469 6d65 275d 203d 2073 656c 662e 7374  Time'] = self.st
+0002cd80: 6172 745f 7469 6d65 0a20 2020 2020 2020  art_time.       
+0002cd90: 2069 6620 7365 6c66 2e73 7461 7475 7320   if self.status 
+0002cda0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002cdb0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002cdc0: 2753 7461 7475 7327 5d20 3d20 7365 6c66  'Status'] = self
+0002cdd0: 2e73 7461 7475 730a 2020 2020 2020 2020  .status.        
+0002cde0: 6966 2073 656c 662e 7465 6e73 6f72 626f  if self.tensorbo
+0002cdf0: 6172 645f 6964 2069 7320 6e6f 7420 4e6f  ard_id is not No
+0002ce00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002ce10: 7265 7375 6c74 5b27 5465 6e73 6f72 626f  result['Tensorbo
+0002ce20: 6172 6449 6427 5d20 3d20 7365 6c66 2e74  ardId'] = self.t
+0002ce30: 656e 736f 7262 6f61 7264 5f69 640a 2020  ensorboard_id.  
+0002ce40: 2020 2020 2020 6966 2073 656c 662e 7665        if self.ve
+0002ce50: 7262 6f73 6520 6973 206e 6f74 204e 6f6e  rbose is not Non
+0002ce60: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002ce70: 6573 756c 745b 2756 6572 626f 7365 275d  esult['Verbose']
+0002ce80: 203d 2073 656c 662e 7665 7262 6f73 650a   = self.verbose.
+0002ce90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002cea0: 776f 726b 7370 6163 655f 6964 2069 7320  workspace_id is 
+0002ceb0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002cec0: 2020 2020 2020 7265 7375 6c74 5b27 576f        result['Wo
+0002ced0: 726b 7370 6163 6549 6427 5d20 3d20 7365  rkspaceId'] = se
+0002cee0: 6c66 2e77 6f72 6b73 7061 6365 5f69 640a  lf.workspace_id.
+0002cef0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002cf00: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0002cf10: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0002cf20: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0002cf30: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0002cf40: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002cf50: 2744 6973 706c 6179 4e61 6d65 2729 2069  'DisplayName') i
+0002cf60: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002cf70: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
+0002cf80: 706c 6179 5f6e 616d 6520 3d20 6d2e 6765  play_name = m.ge
+0002cf90: 7428 2744 6973 706c 6179 4e61 6d65 2729  t('DisplayName')
+0002cfa0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002cfb0: 7428 2745 6e64 5469 6d65 2729 2069 7320  t('EndTime') is 
+0002cfc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002cfd0: 2020 2020 2020 7365 6c66 2e65 6e64 5f74        self.end_t
+0002cfe0: 696d 6520 3d20 6d2e 6765 7428 2745 6e64  ime = m.get('End
+0002cff0: 5469 6d65 2729 0a20 2020 2020 2020 2069  Time').        i
+0002d000: 6620 6d2e 6765 7428 274a 6f62 4964 2729  f m.get('JobId')
+0002d010: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002d020: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
+0002d030: 6f62 5f69 6420 3d20 6d2e 6765 7428 274a  ob_id = m.get('J
+0002d040: 6f62 4964 2729 0a20 2020 2020 2020 2069  obId').        i
+0002d050: 6620 6d2e 6765 7428 274f 7264 6572 2729  f m.get('Order')
+0002d060: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002d070: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
+0002d080: 7264 6572 203d 206d 2e67 6574 2827 4f72  rder = m.get('Or
+0002d090: 6465 7227 290a 2020 2020 2020 2020 6966  der').        if
+0002d0a0: 206d 2e67 6574 2827 5061 6765 4e75 6d62   m.get('PageNumb
+0002d0b0: 6572 2729 2069 7320 6e6f 7420 4e6f 6e65  er') is not None
+0002d0c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002d0d0: 6c66 2e70 6167 655f 6e75 6d62 6572 203d  lf.page_number =
+0002d0e0: 206d 2e67 6574 2827 5061 6765 4e75 6d62   m.get('PageNumb
+0002d0f0: 6572 2729 0a20 2020 2020 2020 2069 6620  er').        if 
+0002d100: 6d2e 6765 7428 2750 6167 6553 697a 6527  m.get('PageSize'
+0002d110: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002d120: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002d130: 7061 6765 5f73 697a 6520 3d20 6d2e 6765  page_size = m.ge
+0002d140: 7428 2750 6167 6553 697a 6527 290a 2020  t('PageSize').  
+0002d150: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002d160: 536f 7274 4279 2729 2069 7320 6e6f 7420  SortBy') is not 
+0002d170: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002d180: 2020 7365 6c66 2e73 6f72 745f 6279 203d    self.sort_by =
+0002d190: 206d 2e67 6574 2827 536f 7274 4279 2729   m.get('SortBy')
+0002d1a0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002d1b0: 7428 2753 6f75 7263 6549 6427 2920 6973  t('SourceId') is
+0002d1c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002d1d0: 2020 2020 2020 2073 656c 662e 736f 7572         self.sour
+0002d1e0: 6365 5f69 6420 3d20 6d2e 6765 7428 2753  ce_id = m.get('S
+0002d1f0: 6f75 7263 6549 6427 290a 2020 2020 2020  ourceId').      
+0002d200: 2020 6966 206d 2e67 6574 2827 536f 7572    if m.get('Sour
+0002d210: 6365 5479 7065 2729 2069 7320 6e6f 7420  ceType') is not 
+0002d220: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002d230: 2020 7365 6c66 2e73 6f75 7263 655f 7479    self.source_ty
+0002d240: 7065 203d 206d 2e67 6574 2827 536f 7572  pe = m.get('Sour
+0002d250: 6365 5479 7065 2729 0a20 2020 2020 2020  ceType').       
+0002d260: 2069 6620 6d2e 6765 7428 2753 7461 7274   if m.get('Start
+0002d270: 5469 6d65 2729 2069 7320 6e6f 7420 4e6f  Time') is not No
+0002d280: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002d290: 7365 6c66 2e73 7461 7274 5f74 696d 6520  self.start_time 
+0002d2a0: 3d20 6d2e 6765 7428 2753 7461 7274 5469  = m.get('StartTi
+0002d2b0: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
+0002d2c0: 6d2e 6765 7428 2753 7461 7475 7327 2920  m.get('Status') 
+0002d2d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002d2e0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+0002d2f0: 6174 7573 203d 206d 2e67 6574 2827 5374  atus = m.get('St
+0002d300: 6174 7573 2729 0a20 2020 2020 2020 2069  atus').        i
+0002d310: 6620 6d2e 6765 7428 2754 656e 736f 7262  f m.get('Tensorb
+0002d320: 6f61 7264 4964 2729 2069 7320 6e6f 7420  oardId') is not 
+0002d330: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002d340: 2020 7365 6c66 2e74 656e 736f 7262 6f61    self.tensorboa
+0002d350: 7264 5f69 6420 3d20 6d2e 6765 7428 2754  rd_id = m.get('T
+0002d360: 656e 736f 7262 6f61 7264 4964 2729 0a20  ensorboardId'). 
+0002d370: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002d380: 2756 6572 626f 7365 2729 2069 7320 6e6f  'Verbose') is no
+0002d390: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002d3a0: 2020 2020 7365 6c66 2e76 6572 626f 7365      self.verbose
+0002d3b0: 203d 206d 2e67 6574 2827 5665 7262 6f73   = m.get('Verbos
+0002d3c0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+0002d3d0: 2e67 6574 2827 576f 726b 7370 6163 6549  .get('WorkspaceI
+0002d3e0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002d3f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002d400: 662e 776f 726b 7370 6163 655f 6964 203d  f.workspace_id =
+0002d410: 206d 2e67 6574 2827 576f 726b 7370 6163   m.get('Workspac
+0002d420: 6549 6427 290a 2020 2020 2020 2020 7265  eId').        re
+0002d430: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0002d440: 7320 4c69 7374 5465 6e73 6f72 626f 6172  s ListTensorboar
+0002d450: 6473 5265 7370 6f6e 7365 426f 6479 2854  dsResponseBody(T
+0002d460: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0002d470: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+0002d480: 2072 6571 7565 7374 5f69 643d 4e6f 6e65   request_id=None
+0002d490: 2c20 7465 6e73 6f72 626f 6172 6473 3d4e  , tensorboards=N
+0002d4a0: 6f6e 652c 2074 6f74 616c 5f63 6f75 6e74  one, total_count
+0002d4b0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0002d4c0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0002d4d0: 3d20 7265 7175 6573 745f 6964 2020 2320  = request_id  # 
+0002d4e0: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
+0002d4f0: 2020 7365 6c66 2e74 656e 736f 7262 6f61    self.tensorboa
+0002d500: 7264 7320 3d20 7465 6e73 6f72 626f 6172  rds = tensorboar
+0002d510: 6473 2020 2320 7479 7065 3a20 6c69 7374  ds  # type: list
+0002d520: 5b54 656e 736f 7262 6f61 7264 5d0a 2020  [Tensorboard].  
+0002d530: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
+0002d540: 5f63 6f75 6e74 203d 2074 6f74 616c 5f63  _count = total_c
+0002d550: 6f75 6e74 2020 2320 7479 7065 3a20 6c6f  ount  # type: lo
+0002d560: 6e67 0a0a 2020 2020 6465 6620 7661 6c69  ng..    def vali
+0002d570: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+0002d580: 2020 2020 6966 2073 656c 662e 7465 6e73      if self.tens
+0002d590: 6f72 626f 6172 6473 3a0a 2020 2020 2020  orboards:.      
+0002d5a0: 2020 2020 2020 666f 7220 6b20 696e 2073        for k in s
+0002d5b0: 656c 662e 7465 6e73 6f72 626f 6172 6473  elf.tensorboards
+0002d5c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0002d5d0: 2020 6966 206b 3a0a 2020 2020 2020 2020    if k:.        
+0002d5e0: 2020 2020 2020 2020 2020 2020 6b2e 7661              k.va
+0002d5f0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+0002d600: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+0002d610: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+0002d620: 7570 6572 284c 6973 7454 656e 736f 7262  uper(ListTensorb
+0002d630: 6f61 7264 7352 6573 706f 6e73 6542 6f64  oardsResponseBod
+0002d640: 792c 2073 656c 6629 2e74 6f5f 6d61 7028  y, self).to_map(
+0002d650: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0002d660: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0002d670: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0002d680: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0002d690: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0002d6a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002d6b0: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
+0002d6c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002d6d0: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
+0002d6e0: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
+0002d6f0: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
+0002d700: 2020 7265 7375 6c74 5b27 5465 6e73 6f72    result['Tensor
+0002d710: 626f 6172 6473 275d 203d 205b 5d0a 2020  boards'] = [].  
+0002d720: 2020 2020 2020 6966 2073 656c 662e 7465        if self.te
+0002d730: 6e73 6f72 626f 6172 6473 2069 7320 6e6f  nsorboards is no
+0002d740: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002d750: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
+0002d760: 662e 7465 6e73 6f72 626f 6172 6473 3a0a  f.tensorboards:.
+0002d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002d780: 7265 7375 6c74 5b27 5465 6e73 6f72 626f  result['Tensorbo
+0002d790: 6172 6473 275d 2e61 7070 656e 6428 6b2e  ards'].append(k.
+0002d7a0: 746f 5f6d 6170 2829 2069 6620 6b20 656c  to_map() if k el
+0002d7b0: 7365 204e 6f6e 6529 0a20 2020 2020 2020  se None).       
+0002d7c0: 2069 6620 7365 6c66 2e74 6f74 616c 5f63   if self.total_c
+0002d7d0: 6f75 6e74 2069 7320 6e6f 7420 4e6f 6e65  ount is not None
+0002d7e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002d7f0: 7375 6c74 5b27 546f 7461 6c43 6f75 6e74  sult['TotalCount
+0002d800: 275d 203d 2073 656c 662e 746f 7461 6c5f  '] = self.total_
+0002d810: 636f 756e 740a 2020 2020 2020 2020 7265  count.        re
+0002d820: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+0002d830: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+0002d840: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+0002d850: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0002d860: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0002d870: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+0002d880: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0002d890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002d8a0: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
+0002d8b0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+0002d8c0: 0a20 2020 2020 2020 2073 656c 662e 7465  .        self.te
+0002d8d0: 6e73 6f72 626f 6172 6473 203d 205b 5d0a  nsorboards = [].
+0002d8e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002d8f0: 2827 5465 6e73 6f72 626f 6172 6473 2729  ('Tensorboards')
+0002d900: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002d910: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+0002d920: 696e 206d 2e67 6574 2827 5465 6e73 6f72  in m.get('Tensor
+0002d930: 626f 6172 6473 2729 3a0a 2020 2020 2020  boards'):.      
+0002d940: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+0002d950: 6f64 656c 203d 2054 656e 736f 7262 6f61  odel = Tensorboa
+0002d960: 7264 2829 0a20 2020 2020 2020 2020 2020  rd().           
+0002d970: 2020 2020 2073 656c 662e 7465 6e73 6f72       self.tensor
+0002d980: 626f 6172 6473 2e61 7070 656e 6428 7465  boards.append(te
+0002d990: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
+0002d9a0: 7028 6b29 290a 2020 2020 2020 2020 6966  p(k)).        if
+0002d9b0: 206d 2e67 6574 2827 546f 7461 6c43 6f75   m.get('TotalCou
+0002d9c0: 6e74 2729 2069 7320 6e6f 7420 4e6f 6e65  nt') is not None
+0002d9d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002d9e0: 6c66 2e74 6f74 616c 5f63 6f75 6e74 203d  lf.total_count =
+0002d9f0: 206d 2e67 6574 2827 546f 7461 6c43 6f75   m.get('TotalCou
+0002da00: 6e74 2729 0a20 2020 2020 2020 2072 6574  nt').        ret
+0002da10: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+0002da20: 204c 6973 7454 656e 736f 7262 6f61 7264   ListTensorboard
+0002da30: 7352 6573 706f 6e73 6528 5465 614d 6f64  sResponse(TeaMod
+0002da40: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+0002da50: 6e69 745f 5f28 7365 6c66 2c20 6865 6164  nit__(self, head
+0002da60: 6572 733d 4e6f 6e65 2c20 7374 6174 7573  ers=None, status
+0002da70: 5f63 6f64 653d 4e6f 6e65 2c20 626f 6479  _code=None, body
+0002da80: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0002da90: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+0002daa0: 6561 6465 7273 2020 2320 7479 7065 3a20  eaders  # type: 
+0002dab0: 6469 6374 5b73 7472 2c20 7374 725d 0a20  dict[str, str]. 
+0002dac0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0002dad0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+0002dae0: 5f63 6f64 6520 2023 2074 7970 653a 2069  _code  # type: i
+0002daf0: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
+0002db00: 626f 6479 203d 2062 6f64 7920 2023 2074  body = body  # t
+0002db10: 7970 653a 204c 6973 7454 656e 736f 7262  ype: ListTensorb
+0002db20: 6f61 7264 7352 6573 706f 6e73 6542 6f64  oardsResponseBod
+0002db30: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+0002db40: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+0002db50: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+0002db60: 5f72 6571 7569 7265 6428 7365 6c66 2e68  _required(self.h
+0002db70: 6561 6465 7273 2c20 2768 6561 6465 7273  eaders, 'headers
+0002db80: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0002db90: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+0002dba0: 6428 7365 6c66 2e73 7461 7475 735f 636f  d(self.status_co
+0002dbb0: 6465 2c20 2773 7461 7475 735f 636f 6465  de, 'status_code
+0002dbc0: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0002dbd0: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+0002dbe0: 6428 7365 6c66 2e62 6f64 792c 2027 626f  d(self.body, 'bo
+0002dbf0: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
+0002dc00: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+0002dc10: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0002dc20: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+0002dc30: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0002dc40: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0002dc50: 3d20 7375 7065 7228 4c69 7374 5465 6e73  = super(ListTens
+0002dc60: 6f72 626f 6172 6473 5265 7370 6f6e 7365  orboardsResponse
+0002dc70: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+0002dc80: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0002dc90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002dca0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002dcb0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0002dcc0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0002dcd0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+0002dce0: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+0002dcf0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002dd00: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+0002dd10: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+0002dd20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002dd30: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+0002dd40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002dd50: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+0002dd60: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+0002dd70: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+0002dd80: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+0002dd90: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+0002dda0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002ddb0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+0002ddc0: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+0002ddd0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002dde0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0002ddf0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0002de00: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0002de10: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0002de20: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002de30: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+0002de40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002de50: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+0002de60: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+0002de70: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+0002de80: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0002de90: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0002dea0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002deb0: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+0002dec0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0002ded0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002dee0: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+0002def0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002df00: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+0002df10: 3d20 4c69 7374 5465 6e73 6f72 626f 6172  = ListTensorboar
+0002df20: 6473 5265 7370 6f6e 7365 426f 6479 2829  dsResponseBody()
+0002df30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002df40: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+0002df50: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+0002df60: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+0002df70: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+0002df80: 6173 7320 5374 6172 7454 656e 736f 7262  ass StartTensorb
+0002df90: 6f61 7264 5265 7175 6573 7428 5465 614d  oardRequest(TeaM
+0002dfa0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0002dfb0: 5f69 6e69 745f 5f28 7365 6c66 2c20 776f  _init__(self, wo
+0002dfc0: 726b 7370 6163 655f 6964 3d4e 6f6e 6529  rkspace_id=None)
+0002dfd0: 3a0a 2020 2020 2020 2020 7365 6c66 2e77  :.        self.w
+0002dfe0: 6f72 6b73 7061 6365 5f69 6420 3d20 776f  orkspace_id = wo
+0002dff0: 726b 7370 6163 655f 6964 2020 2320 7479  rkspace_id  # ty
+0002e000: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
+0002e010: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+0002e020: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+0002e030: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+0002e040: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+0002e050: 7020 3d20 7375 7065 7228 5374 6172 7454  p = super(StartT
+0002e060: 656e 736f 7262 6f61 7264 5265 7175 6573  ensorboardReques
+0002e070: 742c 2073 656c 6629 2e74 6f5f 6d61 7028  t, self).to_map(
+0002e080: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0002e090: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0002e0a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0002e0b0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0002e0c0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0002e0d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002e0e0: 776f 726b 7370 6163 655f 6964 2069 7320  workspace_id is 
+0002e0f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002e100: 2020 2020 2020 7265 7375 6c74 5b27 576f        result['Wo
+0002e110: 726b 7370 6163 6549 6427 5d20 3d20 7365  rkspaceId'] = se
+0002e120: 6c66 2e77 6f72 6b73 7061 6365 5f69 640a  lf.workspace_id.
+0002e130: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002e140: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0002e150: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0002e160: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0002e170: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0002e180: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002e190: 2757 6f72 6b73 7061 6365 4964 2729 2069  'WorkspaceId') i
+0002e1a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002e1b0: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+0002e1c0: 6b73 7061 6365 5f69 6420 3d20 6d2e 6765  kspace_id = m.ge
+0002e1d0: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
+0002e1e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002e1f0: 7365 6c66 0a0a 0a63 6c61 7373 2053 7461  self...class Sta
+0002e200: 7274 5465 6e73 6f72 626f 6172 6452 6573  rtTensorboardRes
+0002e210: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+0002e220: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+0002e230: 6e69 745f 5f28 7365 6c66 2c20 7265 7175  nit__(self, requ
+0002e240: 6573 745f 6964 3d4e 6f6e 652c 2074 656e  est_id=None, ten
+0002e250: 736f 7262 6f61 7264 5f69 643d 4e6f 6e65  sorboard_id=None
+0002e260: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0002e270: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
+0002e280: 7565 7374 5f69 6420 2023 2074 7970 653a  uest_id  # type:
+0002e290: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0002e2a0: 662e 7465 6e73 6f72 626f 6172 645f 6964  f.tensorboard_id
+0002e2b0: 203d 2074 656e 736f 7262 6f61 7264 5f69   = tensorboard_i
+0002e2c0: 6420 2023 2074 7970 653a 2073 7472 0a0a  d  # type: str..
+0002e2d0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0002e2e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002e2f0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+0002e300: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0002e310: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0002e320: 2853 7461 7274 5465 6e73 6f72 626f 6172  (StartTensorboar
+0002e330: 6452 6573 706f 6e73 6542 6f64 792c 2073  dResponseBody, s
+0002e340: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
+0002e350: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+0002e360: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002e370: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+0002e380: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+0002e390: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+0002e3a0: 2020 2020 6966 2073 656c 662e 7265 7175      if self.requ
+0002e3b0: 6573 745f 6964 2069 7320 6e6f 7420 4e6f  est_id is not No
+0002e3c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002e3d0: 7265 7375 6c74 5b27 5265 7175 6573 7449  result['RequestI
+0002e3e0: 6427 5d20 3d20 7365 6c66 2e72 6571 7565  d'] = self.reque
+0002e3f0: 7374 5f69 640a 2020 2020 2020 2020 6966  st_id.        if
+0002e400: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
+0002e410: 645f 6964 2069 7320 6e6f 7420 4e6f 6e65  d_id is not None
+0002e420: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002e430: 7375 6c74 5b27 5465 6e73 6f72 626f 6172  sult['Tensorboar
+0002e440: 6449 6427 5d20 3d20 7365 6c66 2e74 656e  dId'] = self.ten
+0002e450: 736f 7262 6f61 7264 5f69 640a 2020 2020  sorboard_id.    
+0002e460: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0002e470: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+0002e480: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
+0002e490: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0002e4a0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0002e4b0: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
+0002e4c0: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
+0002e4d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002e4e0: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+0002e4f0: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
+0002e500: 7374 4964 2729 0a20 2020 2020 2020 2069  stId').        i
+0002e510: 6620 6d2e 6765 7428 2754 656e 736f 7262  f m.get('Tensorb
+0002e520: 6f61 7264 4964 2729 2069 7320 6e6f 7420  oardId') is not 
+0002e530: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002e540: 2020 7365 6c66 2e74 656e 736f 7262 6f61    self.tensorboa
+0002e550: 7264 5f69 6420 3d20 6d2e 6765 7428 2754  rd_id = m.get('T
+0002e560: 656e 736f 7262 6f61 7264 4964 2729 0a20  ensorboardId'). 
+0002e570: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0002e580: 6c66 0a0a 0a63 6c61 7373 2053 7461 7274  lf...class Start
+0002e590: 5465 6e73 6f72 626f 6172 6452 6573 706f  TensorboardRespo
+0002e5a0: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
+0002e5b0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0002e5c0: 7365 6c66 2c20 6865 6164 6572 733d 4e6f  self, headers=No
+0002e5d0: 6e65 2c20 7374 6174 7573 5f63 6f64 653d  ne, status_code=
+0002e5e0: 4e6f 6e65 2c20 626f 6479 3d4e 6f6e 6529  None, body=None)
+0002e5f0: 3a0a 2020 2020 2020 2020 7365 6c66 2e68  :.        self.h
+0002e600: 6561 6465 7273 203d 2068 6561 6465 7273  eaders = headers
+0002e610: 2020 2320 7479 7065 3a20 6469 6374 5b73    # type: dict[s
+0002e620: 7472 2c20 7374 725d 0a20 2020 2020 2020  tr, str].       
+0002e630: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+0002e640: 6520 3d20 7374 6174 7573 5f63 6f64 6520  e = status_code 
+0002e650: 2023 2074 7970 653a 2069 6e74 0a20 2020   # type: int.   
+0002e660: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+0002e670: 2062 6f64 7920 2023 2074 7970 653a 2053   body  # type: S
+0002e680: 7461 7274 5465 6e73 6f72 626f 6172 6452  tartTensorboardR
+0002e690: 6573 706f 6e73 6542 6f64 790a 0a20 2020  esponseBody..   
+0002e6a0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+0002e6b0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+0002e6c0: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+0002e6d0: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
+0002e6e0: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
+0002e6f0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+0002e700: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+0002e710: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
+0002e720: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
+0002e730: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+0002e740: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+0002e750: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
+0002e760: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+0002e770: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
+0002e780: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
+0002e790: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+0002e7a0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0002e7b0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0002e7c0: 7228 5374 6172 7454 656e 736f 7262 6f61  r(StartTensorboa
+0002e7d0: 7264 5265 7370 6f6e 7365 2c20 7365 6c66  rdResponse, self
+0002e7e0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+0002e7f0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+0002e800: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002e810: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+0002e820: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0002e830: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+0002e840: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+0002e850: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002e860: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002e870: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+0002e880: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+0002e890: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+0002e8a0: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+0002e8b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002e8c0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+0002e8d0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+0002e8e0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+0002e8f0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+0002e900: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002e910: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+0002e920: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+0002e930: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0002e940: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0002e950: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+0002e960: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+0002e970: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+0002e980: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+0002e990: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+0002e9a0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+0002e9b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002e9c0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+0002e9d0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+0002e9e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002e9f0: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+0002ea00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002ea10: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+0002ea20: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+0002ea30: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+0002ea40: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+0002ea50: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+0002ea60: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+0002ea70: 656d 705f 6d6f 6465 6c20 3d20 5374 6172  emp_model = Star
+0002ea80: 7454 656e 736f 7262 6f61 7264 5265 7370  tTensorboardResp
+0002ea90: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+0002eaa0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0002eab0: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+0002eac0: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+0002ead0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0002eae0: 2073 656c 660a 0a0a 636c 6173 7320 5374   self...class St
+0002eaf0: 6f70 4a6f 6252 6573 706f 6e73 6542 6f64  opJobResponseBod
+0002eb00: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+0002eb10: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0002eb20: 6c66 2c20 6a6f 625f 6964 3d4e 6f6e 652c  lf, job_id=None,
+0002eb30: 2072 6571 7565 7374 5f69 643d 4e6f 6e65   request_id=None
+0002eb40: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0002eb50: 6a6f 625f 6964 203d 206a 6f62 5f69 6420  job_id = job_id 
+0002eb60: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+0002eb70: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+0002eb80: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
+0002eb90: 6420 2023 2074 7970 653a 2073 7472 0a0a  d  # type: str..
+0002eba0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0002ebb0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002ebc0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+0002ebd0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0002ebe0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0002ebf0: 2853 746f 704a 6f62 5265 7370 6f6e 7365  (StopJobResponse
+0002ec00: 426f 6479 2c20 7365 6c66 292e 746f 5f6d  Body, self).to_m
+0002ec10: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+0002ec20: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+0002ec30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002ec40: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+0002ec50: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+0002ec60: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0002ec70: 6c66 2e6a 6f62 5f69 6420 6973 206e 6f74  lf.job_id is not
+0002ec80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002ec90: 2020 2072 6573 756c 745b 274a 6f62 4964     result['JobId
+0002eca0: 275d 203d 2073 656c 662e 6a6f 625f 6964  '] = self.job_id
+0002ecb0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002ecc0: 2e72 6571 7565 7374 5f69 6420 6973 206e  .request_id is n
+0002ecd0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002ece0: 2020 2020 2072 6573 756c 745b 2752 6571       result['Req
+0002ecf0: 7565 7374 4964 275d 203d 2073 656c 662e  uestId'] = self.
+0002ed00: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
+0002ed10: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0002ed20: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0002ed30: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+0002ed40: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0002ed50: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0002ed60: 2020 6966 206d 2e67 6574 2827 4a6f 6249    if m.get('JobI
+0002ed70: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002ed80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002ed90: 662e 6a6f 625f 6964 203d 206d 2e67 6574  f.job_id = m.get
+0002eda0: 2827 4a6f 6249 6427 290a 2020 2020 2020  ('JobId').      
+0002edb0: 2020 6966 206d 2e67 6574 2827 5265 7175    if m.get('Requ
+0002edc0: 6573 7449 6427 2920 6973 206e 6f74 204e  estId') is not N
+0002edd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002ede0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+0002edf0: 203d 206d 2e67 6574 2827 5265 7175 6573   = m.get('Reques
+0002ee00: 7449 6427 290a 2020 2020 2020 2020 7265  tId').        re
+0002ee10: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0002ee20: 7320 5374 6f70 4a6f 6252 6573 706f 6e73  s StopJobRespons
+0002ee30: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+0002ee40: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0002ee50: 6c66 2c20 6865 6164 6572 733d 4e6f 6e65  lf, headers=None
+0002ee60: 2c20 7374 6174 7573 5f63 6f64 653d 4e6f  , status_code=No
+0002ee70: 6e65 2c20 626f 6479 3d4e 6f6e 6529 3a0a  ne, body=None):.
+0002ee80: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+0002ee90: 6465 7273 203d 2068 6561 6465 7273 2020  ders = headers  
+0002eea0: 2320 7479 7065 3a20 6469 6374 5b73 7472  # type: dict[str
+0002eeb0: 2c20 7374 725d 0a20 2020 2020 2020 2073  , str].        s
+0002eec0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0002eed0: 3d20 7374 6174 7573 5f63 6f64 6520 2023  = status_code  #
+0002eee0: 2074 7970 653a 2069 6e74 0a20 2020 2020   type: int.     
+0002eef0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+0002ef00: 6f64 7920 2023 2074 7970 653a 2053 746f  ody  # type: Sto
+0002ef10: 704a 6f62 5265 7370 6f6e 7365 426f 6479  pJobResponseBody
+0002ef20: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0002ef30: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0002ef40: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+0002ef50: 7265 7175 6972 6564 2873 656c 662e 6865  required(self.he
+0002ef60: 6164 6572 732c 2027 6865 6164 6572 7327  aders, 'headers'
+0002ef70: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+0002ef80: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+0002ef90: 2873 656c 662e 7374 6174 7573 5f63 6f64  (self.status_cod
+0002efa0: 652c 2027 7374 6174 7573 5f63 6f64 6527  e, 'status_code'
+0002efb0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
+0002efc0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+0002efd0: 2873 656c 662e 626f 6479 2c20 2762 6f64  (self.body, 'bod
+0002efe0: 7927 290a 2020 2020 2020 2020 6966 2073  y').        if s
+0002eff0: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
+0002f000: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
+0002f010: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+0002f020: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+0002f030: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+0002f040: 2073 7570 6572 2853 746f 704a 6f62 5265   super(StopJobRe
+0002f050: 7370 6f6e 7365 2c20 7365 6c66 292e 746f  sponse, self).to
+0002f060: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0002f070: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0002f080: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002f090: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0002f0a0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0002f0b0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0002f0c0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+0002f0d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002f0e0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+0002f0f0: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+0002f100: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+0002f110: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+0002f120: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+0002f130: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002f140: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+0002f150: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+0002f160: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+0002f170: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+0002f180: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002f190: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+0002f1a0: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+0002f1b0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+0002f1c0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+0002f1d0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+0002f1e0: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+0002f1f0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0002f200: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0002f210: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+0002f220: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002f230: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+0002f240: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+0002f250: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+0002f260: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+0002f270: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+0002f280: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002f290: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0002f2a0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+0002f2b0: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+0002f2c0: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+0002f2d0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002f2e0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+0002f2f0: 6d6f 6465 6c20 3d20 5374 6f70 4a6f 6252  model = StopJobR
+0002f300: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
+0002f310: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+0002f320: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+0002f330: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+0002f340: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+0002f350: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+0002f360: 2053 746f 7054 656e 736f 7262 6f61 7264   StopTensorboard
+0002f370: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+0002f380: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0002f390: 745f 5f28 7365 6c66 2c20 776f 726b 7370  t__(self, worksp
+0002f3a0: 6163 655f 6964 3d4e 6f6e 6529 3a0a 2020  ace_id=None):.  
+0002f3b0: 2020 2020 2020 7365 6c66 2e77 6f72 6b73        self.works
+0002f3c0: 7061 6365 5f69 6420 3d20 776f 726b 7370  pace_id = worksp
+0002f3d0: 6163 655f 6964 2020 2320 7479 7065 3a20  ace_id  # type: 
+0002f3e0: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
+0002f3f0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0002f400: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+0002f410: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0002f420: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0002f430: 7375 7065 7228 5374 6f70 5465 6e73 6f72  super(StopTensor
+0002f440: 626f 6172 6452 6571 7565 7374 2c20 7365  boardRequest, se
+0002f450: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+0002f460: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0002f470: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002f480: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0002f490: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0002f4a0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0002f4b0: 2020 2069 6620 7365 6c66 2e77 6f72 6b73     if self.works
+0002f4c0: 7061 6365 5f69 6420 6973 206e 6f74 204e  pace_id is not N
+0002f4d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002f4e0: 2072 6573 756c 745b 2757 6f72 6b73 7061   result['Workspa
+0002f4f0: 6365 4964 275d 203d 2073 656c 662e 776f  ceId'] = self.wo
+0002f500: 726b 7370 6163 655f 6964 0a20 2020 2020  rkspace_id.     
+0002f510: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0002f520: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0002f530: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+0002f540: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0002f550: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0002f560: 2020 6966 206d 2e67 6574 2827 576f 726b    if m.get('Work
+0002f570: 7370 6163 6549 6427 2920 6973 206e 6f74  spaceId') is not
+0002f580: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002f590: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
+0002f5a0: 655f 6964 203d 206d 2e67 6574 2827 576f  e_id = m.get('Wo
+0002f5b0: 726b 7370 6163 6549 6427 290a 2020 2020  rkspaceId').    
+0002f5c0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0002f5d0: 0a0a 636c 6173 7320 5374 6f70 5465 6e73  ..class StopTens
+0002f5e0: 6f72 626f 6172 6452 6573 706f 6e73 6542  orboardResponseB
+0002f5f0: 6f64 7928 5465 614d 6f64 656c 293a 0a20  ody(TeaModel):. 
+0002f600: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0002f610: 7365 6c66 2c20 7265 7175 6573 745f 6964  self, request_id
+0002f620: 3d4e 6f6e 652c 2074 656e 736f 7262 6f61  =None, tensorboa
+0002f630: 7264 5f69 643d 4e6f 6e65 293a 0a20 2020  rd_id=None):.   
+0002f640: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+0002f650: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
+0002f660: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
+0002f670: 2020 2020 2020 2073 656c 662e 7465 6e73         self.tens
+0002f680: 6f72 626f 6172 645f 6964 203d 2074 656e  orboard_id = ten
+0002f690: 736f 7262 6f61 7264 5f69 6420 2023 2074  sorboard_id  # t
+0002f6a0: 7970 653a 2073 7472 0a0a 2020 2020 6465  ype: str..    de
+0002f6b0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+0002f6c0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0002f6d0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+0002f6e0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+0002f6f0: 6170 203d 2073 7570 6572 2853 746f 7054  ap = super(StopT
+0002f700: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
+0002f710: 7365 426f 6479 2c20 7365 6c66 292e 746f  seBody, self).to
+0002f720: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0002f730: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0002f740: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002f750: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0002f760: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0002f770: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0002f780: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0002f790: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002f7a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002f7b0: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+0002f7c0: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+0002f7d0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+0002f7e0: 656e 736f 7262 6f61 7264 5f69 6420 6973  ensorboard_id is
+0002f7f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002f800: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
+0002f810: 656e 736f 7262 6f61 7264 4964 275d 203d  ensorboardId'] =
+0002f820: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
+0002f830: 645f 6964 0a20 2020 2020 2020 2072 6574  d_id.        ret
+0002f840: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0002f850: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0002f860: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+0002f870: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+0002f880: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+0002f890: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+0002f8a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002f8b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002f8c0: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
+0002f8d0: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
+0002f8e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002f8f0: 2827 5465 6e73 6f72 626f 6172 6449 6427  ('TensorboardId'
+0002f900: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002f910: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002f920: 7465 6e73 6f72 626f 6172 645f 6964 203d  tensorboard_id =
+0002f930: 206d 2e67 6574 2827 5465 6e73 6f72 626f   m.get('Tensorbo
+0002f940: 6172 6449 6427 290a 2020 2020 2020 2020  ardId').        
+0002f950: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+0002f960: 6173 7320 5374 6f70 5465 6e73 6f72 626f  ass StopTensorbo
+0002f970: 6172 6452 6573 706f 6e73 6528 5465 614d  ardResponse(TeaM
+0002f980: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0002f990: 5f69 6e69 745f 5f28 7365 6c66 2c20 6865  _init__(self, he
+0002f9a0: 6164 6572 733d 4e6f 6e65 2c20 7374 6174  aders=None, stat
+0002f9b0: 7573 5f63 6f64 653d 4e6f 6e65 2c20 626f  us_code=None, bo
+0002f9c0: 6479 3d4e 6f6e 6529 3a0a 2020 2020 2020  dy=None):.      
+0002f9d0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+0002f9e0: 2068 6561 6465 7273 2020 2320 7479 7065   headers  # type
+0002f9f0: 3a20 6469 6374 5b73 7472 2c20 7374 725d  : dict[str, str]
+0002fa00: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+0002fa10: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
+0002fa20: 7573 5f63 6f64 6520 2023 2074 7970 653a  us_code  # type:
+0002fa30: 2069 6e74 0a20 2020 2020 2020 2073 656c   int.        sel
+0002fa40: 662e 626f 6479 203d 2062 6f64 7920 2023  f.body = body  #
+0002fa50: 2074 7970 653a 2053 746f 7054 656e 736f   type: StopTenso
+0002fa60: 7262 6f61 7264 5265 7370 6f6e 7365 426f  rboardResponseBo
+0002fa70: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
+0002fa80: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+0002fa90: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+0002faa0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+0002fab0: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
+0002fac0: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
+0002fad0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+0002fae0: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
+0002faf0: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
+0002fb00: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
+0002fb10: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+0002fb20: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
+0002fb30: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
+0002fb40: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+0002fb50: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+0002fb60: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+0002fb70: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0002fb80: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0002fb90: 203d 2073 7570 6572 2853 746f 7054 656e   = super(StopTen
+0002fba0: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
+0002fbb0: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+0002fbc0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0002fbd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002fbe0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002fbf0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0002fc00: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0002fc10: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+0002fc20: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+0002fc30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002fc40: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+0002fc50: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+0002fc60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002fc70: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+0002fc80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002fc90: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+0002fca0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+0002fcb0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+0002fcc0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+0002fcd0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+0002fce0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002fcf0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+0002fd00: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+0002fd10: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002fd20: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0002fd30: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0002fd40: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0002fd50: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0002fd60: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002fd70: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+0002fd80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002fd90: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+0002fda0: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+0002fdb0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+0002fdc0: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0002fdd0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0002fde0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002fdf0: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+0002fe00: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0002fe10: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002fe20: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+0002fe30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002fe40: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+0002fe50: 3d20 5374 6f70 5465 6e73 6f72 626f 6172  = StopTensorboar
+0002fe60: 6452 6573 706f 6e73 6542 6f64 7928 290a  dResponseBody().
+0002fe70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002fe80: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
+0002fe90: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
+0002fea0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
+0002feb0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+0002fec0: 7373 2055 7064 6174 654a 6f62 5265 7175  ss UpdateJobRequ
+0002fed0: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+0002fee0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0002fef0: 7365 6c66 2c20 7072 696f 7269 7479 3d4e  self, priority=N
+0002ff00: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+0002ff10: 6c66 2e70 7269 6f72 6974 7920 3d20 7072  lf.priority = pr
+0002ff20: 696f 7269 7479 2020 2320 7479 7065 3a20  iority  # type: 
+0002ff30: 696e 740a 0a20 2020 2064 6566 2076 616c  int..    def val
+0002ff40: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0002ff50: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+0002ff60: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0002ff70: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0002ff80: 7375 7065 7228 5570 6461 7465 4a6f 6252  super(UpdateJobR
+0002ff90: 6571 7565 7374 2c20 7365 6c66 292e 746f  equest, self).to
+0002ffa0: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0002ffb0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0002ffc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002ffd0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0002ffe0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0002fff0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00030000: 7365 6c66 2e70 7269 6f72 6974 7920 6973  self.priority is
+00030010: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00030020: 2020 2020 2020 2072 6573 756c 745b 2750         result['P
+00030030: 7269 6f72 6974 7927 5d20 3d20 7365 6c66  riority'] = self
+00030040: 2e70 7269 6f72 6974 790a 2020 2020 2020  .priority.      
+00030050: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00030060: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00030070: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+00030080: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00030090: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+000300a0: 2069 6620 6d2e 6765 7428 2750 7269 6f72   if m.get('Prior
+000300b0: 6974 7927 2920 6973 206e 6f74 204e 6f6e  ity') is not Non
+000300c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000300d0: 656c 662e 7072 696f 7269 7479 203d 206d  elf.priority = m
+000300e0: 2e67 6574 2827 5072 696f 7269 7479 2729  .get('Priority')
+000300f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00030100: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
+00030110: 6174 654a 6f62 5265 7370 6f6e 7365 426f  ateJobResponseBo
+00030120: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
+00030130: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00030140: 656c 662c 206a 6f62 5f69 643d 4e6f 6e65  elf, job_id=None
+00030150: 2c20 7265 7175 6573 745f 6964 3d4e 6f6e  , request_id=Non
+00030160: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00030170: 2e6a 6f62 5f69 6420 3d20 6a6f 625f 6964  .job_id = job_id
+00030180: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+00030190: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+000301a0: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
+000301b0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+000301c0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+000301d0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000301e0: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+000301f0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00030200: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00030210: 7228 5570 6461 7465 4a6f 6252 6573 706f  r(UpdateJobRespo
+00030220: 6e73 6542 6f64 792c 2073 656c 6629 2e74  nseBody, self).t
+00030230: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00030240: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00030250: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00030260: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00030270: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00030280: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00030290: 2073 656c 662e 6a6f 625f 6964 2069 7320   self.job_id is 
+000302a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000302b0: 2020 2020 2020 7265 7375 6c74 5b27 4a6f        result['Jo
+000302c0: 6249 6427 5d20 3d20 7365 6c66 2e6a 6f62  bId'] = self.job
+000302d0: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+000302e0: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
+000302f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00030300: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00030310: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
+00030320: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
+00030330: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00030340: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00030350: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+00030360: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00030370: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00030380: 2020 2020 2069 6620 6d2e 6765 7428 274a       if m.get('J
+00030390: 6f62 4964 2729 2069 7320 6e6f 7420 4e6f  obId') is not No
+000303a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000303b0: 7365 6c66 2e6a 6f62 5f69 6420 3d20 6d2e  self.job_id = m.
+000303c0: 6765 7428 274a 6f62 4964 2729 0a20 2020  get('JobId').   
+000303d0: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+000303e0: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
+000303f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00030400: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+00030410: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
+00030420: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
+00030430: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+00030440: 6c61 7373 2055 7064 6174 654a 6f62 5265  lass UpdateJobRe
+00030450: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+00030460: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00030470: 5f5f 2873 656c 662c 2068 6561 6465 7273  __(self, headers
+00030480: 3d4e 6f6e 652c 2073 7461 7475 735f 636f  =None, status_co
+00030490: 6465 3d4e 6f6e 652c 2062 6f64 793d 4e6f  de=None, body=No
+000304a0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+000304b0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+000304c0: 6572 7320 2023 2074 7970 653a 2064 6963  ers  # type: dic
+000304d0: 745b 7374 722c 2073 7472 5d0a 2020 2020  t[str, str].    
+000304e0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+000304f0: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+00030500: 6465 2020 2320 7479 7065 3a20 696e 740a  de  # type: int.
+00030510: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00030520: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
+00030530: 3a20 5570 6461 7465 4a6f 6252 6573 706f  : UpdateJobRespo
+00030540: 6e73 6542 6f64 790a 0a20 2020 2064 6566  nseBody..    def
+00030550: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00030560: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00030570: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+00030580: 7365 6c66 2e68 6561 6465 7273 2c20 2768  self.headers, 'h
+00030590: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+000305a0: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+000305b0: 6571 7569 7265 6428 7365 6c66 2e73 7461  equired(self.sta
+000305c0: 7475 735f 636f 6465 2c20 2773 7461 7475  tus_code, 'statu
+000305d0: 735f 636f 6465 2729 0a20 2020 2020 2020  s_code').       
+000305e0: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+000305f0: 6571 7569 7265 6428 7365 6c66 2e62 6f64  equired(self.bod
+00030600: 792c 2027 626f 6479 2729 0a20 2020 2020  y, 'body').     
+00030610: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+00030620: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00030630: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+00030640: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+00030650: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00030660: 205f 6d61 7020 3d20 7375 7065 7228 5570   _map = super(Up
+00030670: 6461 7465 4a6f 6252 6573 706f 6e73 652c  dateJobResponse,
+00030680: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
+00030690: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+000306a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000306b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000306c0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+000306d0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+000306e0: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+000306f0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+00030700: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00030710: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+00030720: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+00030730: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00030740: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+00030750: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00030760: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+00030770: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+00030780: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+00030790: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+000307a0: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+000307b0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000307c0: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+000307d0: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+000307e0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000307f0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+00030800: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
+00030810: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+00030820: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+00030830: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00030840: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+00030850: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00030860: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+00030870: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+00030880: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00030890: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+000308a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000308b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000308c0: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+000308d0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+000308e0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000308f0: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
+00030900: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00030910: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+00030920: 2055 7064 6174 654a 6f62 5265 7370 6f6e   UpdateJobRespon
+00030930: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
+00030940: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+00030950: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+00030960: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+00030970: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00030980: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
+00030990: 7465 5465 6e73 6f72 626f 6172 6452 6571  teTensorboardReq
+000309a0: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+000309b0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+000309c0: 2873 656c 662c 206d 6178 5f72 756e 6e69  (self, max_runni
+000309d0: 6e67 5f74 696d 655f 6d69 6e75 7465 733d  ng_time_minutes=
+000309e0: 4e6f 6e65 2c20 776f 726b 7370 6163 655f  None, workspace_
+000309f0: 6964 3d4e 6f6e 6529 3a0a 2020 2020 2020  id=None):.      
+00030a00: 2020 7365 6c66 2e6d 6178 5f72 756e 6e69    self.max_runni
+00030a10: 6e67 5f74 696d 655f 6d69 6e75 7465 7320  ng_time_minutes 
+00030a20: 3d20 6d61 785f 7275 6e6e 696e 675f 7469  = max_running_ti
+00030a30: 6d65 5f6d 696e 7574 6573 2020 2320 7479  me_minutes  # ty
+00030a40: 7065 3a20 6c6f 6e67 0a20 2020 2020 2020  pe: long.       
+00030a50: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
+00030a60: 6964 203d 2077 6f72 6b73 7061 6365 5f69  id = workspace_i
+00030a70: 6420 2023 2074 7970 653a 2073 7472 0a0a  d  # type: str..
+00030a80: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00030a90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00030aa0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+00030ab0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00030ac0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00030ad0: 2855 7064 6174 6554 656e 736f 7262 6f61  (UpdateTensorboa
+00030ae0: 7264 5265 7175 6573 742c 2073 656c 6629  rdRequest, self)
+00030af0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00030b00: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00030b10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00030b20: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00030b30: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00030b40: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00030b50: 6966 2073 656c 662e 6d61 785f 7275 6e6e  if self.max_runn
+00030b60: 696e 675f 7469 6d65 5f6d 696e 7574 6573  ing_time_minutes
+00030b70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00030b80: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00030b90: 5b27 4d61 7852 756e 6e69 6e67 5469 6d65  ['MaxRunningTime
+00030ba0: 4d69 6e75 7465 7327 5d20 3d20 7365 6c66  Minutes'] = self
+00030bb0: 2e6d 6178 5f72 756e 6e69 6e67 5f74 696d  .max_running_tim
+00030bc0: 655f 6d69 6e75 7465 730a 2020 2020 2020  e_minutes.      
+00030bd0: 2020 6966 2073 656c 662e 776f 726b 7370    if self.worksp
+00030be0: 6163 655f 6964 2069 7320 6e6f 7420 4e6f  ace_id is not No
+00030bf0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00030c00: 7265 7375 6c74 5b27 576f 726b 7370 6163  result['Workspac
+00030c10: 6549 6427 5d20 3d20 7365 6c66 2e77 6f72  eId'] = self.wor
+00030c20: 6b73 7061 6365 5f69 640a 2020 2020 2020  kspace_id.      
+00030c30: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00030c40: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00030c50: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+00030c60: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00030c70: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00030c80: 2069 6620 6d2e 6765 7428 274d 6178 5275   if m.get('MaxRu
+00030c90: 6e6e 696e 6754 696d 654d 696e 7574 6573  nningTimeMinutes
+00030ca0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00030cb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00030cc0: 2e6d 6178 5f72 756e 6e69 6e67 5f74 696d  .max_running_tim
+00030cd0: 655f 6d69 6e75 7465 7320 3d20 6d2e 6765  e_minutes = m.ge
+00030ce0: 7428 274d 6178 5275 6e6e 696e 6754 696d  t('MaxRunningTim
+00030cf0: 654d 696e 7574 6573 2729 0a20 2020 2020  eMinutes').     
+00030d00: 2020 2069 6620 6d2e 6765 7428 2757 6f72     if m.get('Wor
+00030d10: 6b73 7061 6365 4964 2729 2069 7320 6e6f  kspaceId') is no
+00030d20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00030d30: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
+00030d40: 6365 5f69 6420 3d20 6d2e 6765 7428 2757  ce_id = m.get('W
+00030d50: 6f72 6b73 7061 6365 4964 2729 0a20 2020  orkspaceId').   
+00030d60: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00030d70: 0a0a 0a63 6c61 7373 2055 7064 6174 6554  ...class UpdateT
+00030d80: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
+00030d90: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
+00030da0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00030db0: 5f5f 2873 656c 662c 2072 6571 7565 7374  __(self, request
+00030dc0: 5f69 643d 4e6f 6e65 2c20 7465 6e73 6f72  _id=None, tensor
+00030dd0: 626f 6172 645f 6964 3d4e 6f6e 6529 3a0a  board_id=None):.
+00030de0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+00030df0: 7565 7374 5f69 6420 3d20 7265 7175 6573  uest_id = reques
+00030e00: 745f 6964 2020 2320 7479 7065 3a20 7374  t_id  # type: st
+00030e10: 720a 2020 2020 2020 2020 7365 6c66 2e74  r.        self.t
+00030e20: 656e 736f 7262 6f61 7264 5f69 6420 3d20  ensorboard_id = 
+00030e30: 7465 6e73 6f72 626f 6172 645f 6964 2020  tensorboard_id  
+00030e40: 2320 7479 7065 3a20 7374 720a 0a20 2020  # type: str..   
+00030e50: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00030e60: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00030e70: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+00030e80: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00030e90: 205f 6d61 7020 3d20 7375 7065 7228 5570   _map = super(Up
+00030ea0: 6461 7465 5465 6e73 6f72 626f 6172 6452  dateTensorboardR
+00030eb0: 6573 706f 6e73 6542 6f64 792c 2073 656c  esponseBody, sel
+00030ec0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
+00030ed0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00030ee0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00030ef0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00030f00: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00030f10: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00030f20: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
+00030f30: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
+00030f40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00030f50: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
+00030f60: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
+00030f70: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00030f80: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
+00030f90: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00030fa0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00030fb0: 6c74 5b27 5465 6e73 6f72 626f 6172 6449  lt['TensorboardI
+00030fc0: 6427 5d20 3d20 7365 6c66 2e74 656e 736f  d'] = self.tenso
+00030fd0: 7262 6f61 7264 5f69 640a 2020 2020 2020  rboard_id.      
+00030fe0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00030ff0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00031000: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+00031010: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00031020: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00031030: 2069 6620 6d2e 6765 7428 2752 6571 7565   if m.get('Reque
+00031040: 7374 4964 2729 2069 7320 6e6f 7420 4e6f  stId') is not No
+00031050: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00031060: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00031070: 3d20 6d2e 6765 7428 2752 6571 7565 7374  = m.get('Request
+00031080: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+00031090: 6d2e 6765 7428 2754 656e 736f 7262 6f61  m.get('Tensorboa
+000310a0: 7264 4964 2729 2069 7320 6e6f 7420 4e6f  rdId') is not No
+000310b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000310c0: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
+000310d0: 5f69 6420 3d20 6d2e 6765 7428 2754 656e  _id = m.get('Ten
+000310e0: 736f 7262 6f61 7264 4964 2729 0a20 2020  sorboardId').   
+000310f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00031100: 0a0a 0a63 6c61 7373 2055 7064 6174 6554  ...class UpdateT
+00031110: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
+00031120: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+00031130: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00031140: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
+00031150: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
+00031160: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
+00031170: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+00031180: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
+00031190: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
+000311a0: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
+000311b0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+000311c0: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
+000311d0: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
+000311e0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+000311f0: 626f 6479 2020 2320 7479 7065 3a20 5570  body  # type: Up
+00031200: 6461 7465 5465 6e73 6f72 626f 6172 6452  dateTensorboardR
+00031210: 6573 706f 6e73 6542 6f64 790a 0a20 2020  esponseBody..   
+00031220: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00031230: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+00031240: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00031250: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
+00031260: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
+00031270: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+00031280: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+00031290: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
+000312a0: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
+000312b0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+000312c0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+000312d0: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
+000312e0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+000312f0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
+00031300: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
+00031310: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+00031320: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00031330: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00031340: 7228 5570 6461 7465 5465 6e73 6f72 626f  r(UpdateTensorbo
+00031350: 6172 6452 6573 706f 6e73 652c 2073 656c  ardResponse, sel
+00031360: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
+00031370: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00031380: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00031390: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+000313a0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+000313b0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+000313c0: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+000313d0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+000313e0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000313f0: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+00031400: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+00031410: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00031420: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+00031430: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00031440: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+00031450: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+00031460: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+00031470: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+00031480: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00031490: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+000314a0: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+000314b0: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+000314c0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+000314d0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+000314e0: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+000314f0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00031500: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00031510: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+00031520: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+00031530: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00031540: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+00031550: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+00031560: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00031570: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+00031580: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00031590: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+000315a0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+000315b0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+000315c0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000315d0: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+000315e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000315f0: 7465 6d70 5f6d 6f64 656c 203d 2055 7064  temp_model = Upd
+00031600: 6174 6554 656e 736f 7262 6f61 7264 5265  ateTensorboardRe
+00031610: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
+00031620: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+00031630: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+00031640: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+00031650: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+00031660: 726e 2073 656c 660a 0a0a                 rn self...
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.7/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO` & `alibabacloud_pai-dlc20201203_py2-1.2.8/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pai-dlc20201203-py2
-Version: 1.2.7
+Version: 1.2.8
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.7/setup.py` & `alibabacloud_pai-dlc20201203_py2-1.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pai-dlc20201203_py2.
 
-Created on 21/07/2023
+Created on 26/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pai_dlc20201203"
 NAME = "alibabacloud_pai-dlc20201203_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud pai-dlc (20201203) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

