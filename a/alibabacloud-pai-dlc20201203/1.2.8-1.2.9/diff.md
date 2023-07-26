# Comparing `tmp/alibabacloud_pai-dlc20201203-1.2.8.tar.gz` & `tmp/alibabacloud_pai-dlc20201203-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pai-dlc20201203-1.2.8.tar", last modified: Fri Jul 21 13:06:17 2023, max compression
+gzip compressed data, was "dist/alibabacloud_pai-dlc20201203-1.2.9.tar", last modified: Wed Jul 26 11:30:26 2023, max compression
```

## Comparing `alibabacloud_pai-dlc20201203-1.2.8.tar` & `alibabacloud_pai-dlc20201203-1.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:06:17.000000 alibabacloud_pai-dlc20201203-1.2.8/
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-21 13:06:16.000000 alibabacloud_pai-dlc20201203-1.2.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-21 13:06:16.000000 alibabacloud_pai-dlc20201203-1.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-21 13:06:16.000000 alibabacloud_pai-dlc20201203-1.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2023-07-21 13:06:17.000000 alibabacloud_pai-dlc20201203-1.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2023-07-21 13:06:16.000000 alibabacloud_pai-dlc20201203-1.2.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-07-21 13:06:16.000000 alibabacloud_pai-dlc20201203-1.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:06:17.000000 alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-21 13:06:16.000000 alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76692 2023-07-21 13:06:16.000000 alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203/client.py
--rw-r--r--   0 root         (0) root         (0)   199211 2023-07-21 13:06:16.000000 alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 13:06:17.000000 alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2023-07-21 13:06:17.000000 alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2023-07-21 13:06:17.000000 alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 13:06:17.000000 alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-21 13:06:17.000000 alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-21 13:06:17.000000 alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-21 13:06:17.000000 alibabacloud_pai-dlc20201203-1.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2633 2023-07-21 13:06:16.000000 alibabacloud_pai-dlc20201203-1.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/
+-rw-r--r--   0 root         (0) root         (0)      918 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79766 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203/client.py
+-rw-r--r--   0 root         (0) root         (0)   202496 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-07-26 11:30:26.000000 alibabacloud_pai-dlc20201203-1.2.9/setup.py
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.8/ChangeLog.md` & `alibabacloud_pai-dlc20201203-1.2.9/ChangeLog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-21 Version: 1.2.8
+- Change the API -- GetWebTerminal.
+
 2023-07-19 Version: 1.2.7
 - Open the API.
 
 2023-05-26 Version: 1.2.6
 - Add parameter in JobElasticSpec.
 
 2023-03-23 Version: 1.2.5
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.8/LICENSE` & `alibabacloud_pai-dlc20201203-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.2.8/PKG-INFO` & `alibabacloud_pai-dlc20201203-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pai-dlc20201203
-Version: 1.2.8
+Version: 1.2.9
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.8/README-CN.md` & `alibabacloud_pai-dlc20201203-1.2.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.2.8/README.md` & `alibabacloud_pai-dlc20201203-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203/client.py` & `alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1059,14 +1059,98 @@
         tensorboard_id: str,
         request: pai_dlc_20201203_models.GetTensorboardRequest,
     ) -> pai_dlc_20201203_models.GetTensorboardResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_tensorboard_with_options_async(tensorboard_id, request, headers, runtime)
 
+    def get_token_with_options(
+        self,
+        request: pai_dlc_20201203_models.GetTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_dlc_20201203_models.GetTokenResponse:
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
+            pathname=f'/api/v1/tokens',
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
+    async def get_token_with_options_async(
+        self,
+        request: pai_dlc_20201203_models.GetTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_dlc_20201203_models.GetTokenResponse:
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
+            pathname=f'/api/v1/tokens',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_dlc_20201203_models.GetTokenResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_token(
+        self,
+        request: pai_dlc_20201203_models.GetTokenRequest,
+    ) -> pai_dlc_20201203_models.GetTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_token_with_options(request, headers, runtime)
+
+    async def get_token_async(
+        self,
+        request: pai_dlc_20201203_models.GetTokenRequest,
+    ) -> pai_dlc_20201203_models.GetTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_token_with_options_async(request, headers, runtime)
+
     def get_web_terminal_with_options(
         self,
         job_id: str,
         pod_id: str,
         request: pai_dlc_20201203_models.GetWebTerminalRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203/models.py` & `alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9924,2528 +9924,2733 @@
 00026c30: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
 00026c40: 6f64 656c 203d 2054 656e 736f 7262 6f61  odel = Tensorboa
 00026c50: 7264 2829 0a20 2020 2020 2020 2020 2020  rd().           
 00026c60: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
 00026c70: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
 00026c80: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
 00026c90: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00026ca0: 0a0a 636c 6173 7320 4765 7457 6562 5465  ..class GetWebTe
-00026cb0: 726d 696e 616c 5265 7175 6573 7428 5465  rminalRequest(Te
-00026cc0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00026cd0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00026ce0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00026cf0: 2070 6f64 5f75 6964 3a20 7374 7220 3d20   pod_uid: str = 
-00026d00: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00026d10: 2020 2020 2023 2050 6f64 2055 4944 e380       # Pod UID..
-00026d20: 820a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-00026d30: 6f64 5f75 6964 203d 2070 6f64 5f75 6964  od_uid = pod_uid
-00026d40: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00026d50: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00026d60: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00026d70: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00026d80: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00026d90: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-00026da0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-00026db0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00026dc0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-00026dd0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-00026de0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-00026df0: 2020 2020 6966 2073 656c 662e 706f 645f      if self.pod_
-00026e00: 7569 6420 6973 206e 6f74 204e 6f6e 653a  uid is not None:
-00026e10: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00026e20: 756c 745b 2750 6f64 5569 6427 5d20 3d20  ult['PodUid'] = 
-00026e30: 7365 6c66 2e70 6f64 5f75 6964 0a20 2020  self.pod_uid.   
-00026e40: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00026e50: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-00026e60: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-00026e70: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-00026e80: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-00026e90: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-00026ea0: 2e67 6574 2827 506f 6455 6964 2729 2069  .get('PodUid') i
-00026eb0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00026ec0: 2020 2020 2020 2020 7365 6c66 2e70 6f64          self.pod
-00026ed0: 5f75 6964 203d 206d 2e67 6574 2827 506f  _uid = m.get('Po
-00026ee0: 6455 6964 2729 0a20 2020 2020 2020 2072  dUid').        r
-00026ef0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-00026f00: 7373 2047 6574 5765 6254 6572 6d69 6e61  ss GetWebTermina
-00026f10: 6c52 6573 706f 6e73 6542 6f64 7928 5465  lResponseBody(Te
-00026f20: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00026f30: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00026f40: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00026f50: 2072 6571 7565 7374 5f69 643a 2073 7472   request_id: str
-00026f60: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00026f70: 2077 6562 5f74 6572 6d69 6e61 6c5f 7572   web_terminal_ur
-00026f80: 6c3a 2073 7472 203d 204e 6f6e 652c 0a20  l: str = None,. 
-00026f90: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-00026fa0: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-00026fb0: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
-00026fc0: 2020 2073 656c 662e 7765 625f 7465 726d     self.web_term
-00026fd0: 696e 616c 5f75 726c 203d 2077 6562 5f74  inal_url = web_t
-00026fe0: 6572 6d69 6e61 6c5f 7572 6c0a 0a20 2020  erminal_url..   
-00026ff0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-00027000: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-00027010: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-00027020: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00027030: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-00027040: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00027050: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00027060: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00027070: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00027080: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00027090: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-000270a0: 6620 7365 6c66 2e72 6571 7565 7374 5f69  f self.request_i
-000270b0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-000270c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000270d0: 745b 2752 6571 7565 7374 4964 275d 203d  t['RequestId'] =
-000270e0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-000270f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00027100: 2e77 6562 5f74 6572 6d69 6e61 6c5f 7572  .web_terminal_ur
-00027110: 6c20 6973 206e 6f74 204e 6f6e 653a 0a20  l is not None:. 
-00027120: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00027130: 745b 2757 6562 5465 726d 696e 616c 5572  t['WebTerminalUr
-00027140: 6c27 5d20 3d20 7365 6c66 2e77 6562 5f74  l'] = self.web_t
-00027150: 6572 6d69 6e61 6c5f 7572 6c0a 2020 2020  erminal_url.    
-00027160: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00027170: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00027180: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-00027190: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-000271a0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-000271b0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-000271c0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-000271d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000271e0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000271f0: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
-00027200: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
-00027210: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00027220: 2757 6562 5465 726d 696e 616c 5572 6c27  'WebTerminalUrl'
-00027230: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00027240: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00027250: 7765 625f 7465 726d 696e 616c 5f75 726c  web_terminal_url
-00027260: 203d 206d 2e67 6574 2827 5765 6254 6572   = m.get('WebTer
-00027270: 6d69 6e61 6c55 726c 2729 0a20 2020 2020  minalUrl').     
-00027280: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00027290: 0a63 6c61 7373 2047 6574 5765 6254 6572  .class GetWebTer
-000272a0: 6d69 6e61 6c52 6573 706f 6e73 6528 5465  minalResponse(Te
-000272b0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-000272c0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-000272d0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-000272e0: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
-000272f0: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
-00027300: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
-00027310: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
-00027320: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
-00027330: 4765 7457 6562 5465 726d 696e 616c 5265  GetWebTerminalRe
-00027340: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
-00027350: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00027360: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-00027370: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
-00027380: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00027390: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
-000273a0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-000273b0: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
-000273c0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-000273d0: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
-000273e0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
-000273f0: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
-00027400: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-00027410: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
-00027420: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
-00027430: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
-00027440: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
-00027450: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
-00027460: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
-00027470: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
-00027480: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-00027490: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000274a0: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
-000274b0: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-000274c0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-000274d0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-000274e0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-000274f0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-00027500: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00027510: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-00027520: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00027530: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00027540: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-00027550: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00027560: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00027570: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-00027580: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-00027590: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-000275a0: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-000275b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000275c0: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-000275d0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-000275e0: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-000275f0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-00027600: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00027610: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-00027620: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-00027630: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-00027640: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00027650: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-00027660: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-00027670: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-00027680: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00027690: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000276a0: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
-000276b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000276c0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-000276d0: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
-000276e0: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
-000276f0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-00027700: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00027710: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00027720: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-00027730: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-00027740: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-00027750: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
-00027760: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00027770: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-00027780: 203d 2047 6574 5765 6254 6572 6d69 6e61   = GetWebTermina
-00027790: 6c52 6573 706f 6e73 6542 6f64 7928 290a  lResponseBody().
-000277a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000277b0: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-000277c0: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-000277d0: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-000277e0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-000277f0: 7373 204c 6973 7445 6373 5370 6563 7352  ss ListEcsSpecsR
-00027800: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-00027810: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00027820: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-00027830: 2c0a 2020 2020 2020 2020 6163 6365 6c65  ,.        accele
-00027840: 7261 746f 725f 7479 7065 3a20 7374 7220  rator_type: str 
-00027850: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00027860: 6f72 6465 723a 2073 7472 203d 204e 6f6e  order: str = Non
-00027870: 652c 0a20 2020 2020 2020 2070 6167 655f  e,.        page_
-00027880: 6e75 6d62 6572 3a20 696e 7420 3d20 4e6f  number: int = No
-00027890: 6e65 2c0a 2020 2020 2020 2020 7061 6765  ne,.        page
-000278a0: 5f73 697a 653a 2069 6e74 203d 204e 6f6e  _size: int = Non
-000278b0: 652c 0a20 2020 2020 2020 2073 6f72 745f  e,.        sort_
-000278c0: 6279 3a20 7374 7220 3d20 4e6f 6e65 2c0a  by: str = None,.
-000278d0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-000278e0: 656c 662e 6163 6365 6c65 7261 746f 725f  elf.accelerator_
-000278f0: 7479 7065 203d 2061 6363 656c 6572 6174  type = accelerat
-00027900: 6f72 5f74 7970 650a 2020 2020 2020 2020  or_type.        
-00027910: 7365 6c66 2e6f 7264 6572 203d 206f 7264  self.order = ord
-00027920: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
-00027930: 7061 6765 5f6e 756d 6265 7220 3d20 7061  page_number = pa
-00027940: 6765 5f6e 756d 6265 720a 2020 2020 2020  ge_number.      
-00027950: 2020 7365 6c66 2e70 6167 655f 7369 7a65    self.page_size
-00027960: 203d 2070 6167 655f 7369 7a65 0a20 2020   = page_size.   
-00027970: 2020 2020 2073 656c 662e 736f 7274 5f62       self.sort_b
-00027980: 7920 3d20 736f 7274 5f62 790a 0a20 2020  y = sort_by..   
-00027990: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-000279a0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-000279b0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-000279c0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-000279d0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-000279e0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-000279f0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-00027a00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00027a10: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-00027a20: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00027a30: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-00027a40: 6620 7365 6c66 2e61 6363 656c 6572 6174  f self.accelerat
-00027a50: 6f72 5f74 7970 6520 6973 206e 6f74 204e  or_type is not N
-00027a60: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00027a70: 2072 6573 756c 745b 2741 6363 656c 6572   result['Acceler
-00027a80: 6174 6f72 5479 7065 275d 203d 2073 656c  atorType'] = sel
-00027a90: 662e 6163 6365 6c65 7261 746f 725f 7479  f.accelerator_ty
-00027aa0: 7065 0a20 2020 2020 2020 2069 6620 7365  pe.        if se
-00027ab0: 6c66 2e6f 7264 6572 2069 7320 6e6f 7420  lf.order is not 
-00027ac0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00027ad0: 2020 7265 7375 6c74 5b27 4f72 6465 7227    result['Order'
-00027ae0: 5d20 3d20 7365 6c66 2e6f 7264 6572 0a20  ] = self.order. 
-00027af0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00027b00: 6167 655f 6e75 6d62 6572 2069 7320 6e6f  age_number is no
-00027b10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00027b20: 2020 2020 7265 7375 6c74 5b27 5061 6765      result['Page
-00027b30: 4e75 6d62 6572 275d 203d 2073 656c 662e  Number'] = self.
-00027b40: 7061 6765 5f6e 756d 6265 720a 2020 2020  page_number.    
-00027b50: 2020 2020 6966 2073 656c 662e 7061 6765      if self.page
-00027b60: 5f73 697a 6520 6973 206e 6f74 204e 6f6e  _size is not Non
-00027b70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00027b80: 6573 756c 745b 2750 6167 6553 697a 6527  esult['PageSize'
-00027b90: 5d20 3d20 7365 6c66 2e70 6167 655f 7369  ] = self.page_si
-00027ba0: 7a65 0a20 2020 2020 2020 2069 6620 7365  ze.        if se
-00027bb0: 6c66 2e73 6f72 745f 6279 2069 7320 6e6f  lf.sort_by is no
-00027bc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00027bd0: 2020 2020 7265 7375 6c74 5b27 536f 7274      result['Sort
-00027be0: 4279 275d 203d 2073 656c 662e 736f 7274  By'] = self.sort
-00027bf0: 5f62 790a 2020 2020 2020 2020 7265 7475  _by.        retu
-00027c00: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00027c10: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00027c20: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-00027c30: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00027c40: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00027c50: 2020 2069 6620 6d2e 6765 7428 2741 6363     if m.get('Acc
-00027c60: 656c 6572 6174 6f72 5479 7065 2729 2069  eleratorType') i
-00027c70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00027c80: 2020 2020 2020 2020 7365 6c66 2e61 6363          self.acc
-00027c90: 656c 6572 6174 6f72 5f74 7970 6520 3d20  elerator_type = 
-00027ca0: 6d2e 6765 7428 2741 6363 656c 6572 6174  m.get('Accelerat
-00027cb0: 6f72 5479 7065 2729 0a20 2020 2020 2020  orType').       
-00027cc0: 2069 6620 6d2e 6765 7428 274f 7264 6572   if m.get('Order
-00027cd0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00027ce0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00027cf0: 2e6f 7264 6572 203d 206d 2e67 6574 2827  .order = m.get('
-00027d00: 4f72 6465 7227 290a 2020 2020 2020 2020  Order').        
-00027d10: 6966 206d 2e67 6574 2827 5061 6765 4e75  if m.get('PageNu
-00027d20: 6d62 6572 2729 2069 7320 6e6f 7420 4e6f  mber') is not No
-00027d30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00027d40: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
-00027d50: 203d 206d 2e67 6574 2827 5061 6765 4e75   = m.get('PageNu
-00027d60: 6d62 6572 2729 0a20 2020 2020 2020 2069  mber').        i
-00027d70: 6620 6d2e 6765 7428 2750 6167 6553 697a  f m.get('PageSiz
-00027d80: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00027d90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00027da0: 662e 7061 6765 5f73 697a 6520 3d20 6d2e  f.page_size = m.
-00027db0: 6765 7428 2750 6167 6553 697a 6527 290a  get('PageSize').
-00027dc0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00027dd0: 2827 536f 7274 4279 2729 2069 7320 6e6f  ('SortBy') is no
-00027de0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00027df0: 2020 2020 7365 6c66 2e73 6f72 745f 6279      self.sort_by
-00027e00: 203d 206d 2e67 6574 2827 536f 7274 4279   = m.get('SortBy
-00027e10: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00027e20: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
-00027e30: 6973 7445 6373 5370 6563 7352 6573 706f  istEcsSpecsRespo
-00027e40: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
-00027e50: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00027e60: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00027e70: 662c 0a20 2020 2020 2020 2065 6373 5f73  f,.        ecs_s
-00027e80: 7065 6373 3a20 4c69 7374 5b45 6373 5370  pecs: List[EcsSp
-00027e90: 6563 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ec] = None,.    
-00027ea0: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
-00027eb0: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00027ec0: 2020 2020 746f 7461 6c5f 636f 756e 743a      total_count:
-00027ed0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-00027ee0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-00027ef0: 2e65 6373 5f73 7065 6373 203d 2065 6373  .ecs_specs = ecs
-00027f00: 5f73 7065 6373 0a20 2020 2020 2020 2073  _specs.        s
-00027f10: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-00027f20: 2072 6571 7565 7374 5f69 640a 2020 2020   request_id.    
-00027f30: 2020 2020 7365 6c66 2e74 6f74 616c 5f63      self.total_c
-00027f40: 6f75 6e74 203d 2074 6f74 616c 5f63 6f75  ount = total_cou
-00027f50: 6e74 0a0a 2020 2020 6465 6620 7661 6c69  nt..    def vali
-00027f60: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-00027f70: 2020 2020 6966 2073 656c 662e 6563 735f      if self.ecs_
-00027f80: 7370 6563 733a 0a20 2020 2020 2020 2020  specs:.         
-00027f90: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
-00027fa0: 2e65 6373 5f73 7065 6373 3a0a 2020 2020  .ecs_specs:.    
-00027fb0: 2020 2020 2020 2020 2020 2020 6966 206b              if k
-00027fc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00027fd0: 2020 2020 2020 6b2e 7661 6c69 6461 7465        k.validate
-00027fe0: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-00027ff0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-00028000: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-00028010: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-00028020: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-00028030: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00028040: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-00028050: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00028060: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00028070: 7265 7375 6c74 5b27 4563 7353 7065 6373  result['EcsSpecs
-00028080: 275d 203d 205b 5d0a 2020 2020 2020 2020  '] = [].        
-00028090: 6966 2073 656c 662e 6563 735f 7370 6563  if self.ecs_spec
-000280a0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-000280b0: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-000280c0: 2069 6e20 7365 6c66 2e65 6373 5f73 7065   in self.ecs_spe
-000280d0: 6373 3a0a 2020 2020 2020 2020 2020 2020  cs:.            
-000280e0: 2020 2020 7265 7375 6c74 5b27 4563 7353      result['EcsS
-000280f0: 7065 6373 275d 2e61 7070 656e 6428 6b2e  pecs'].append(k.
-00028100: 746f 5f6d 6170 2829 2069 6620 6b20 656c  to_map() if k el
-00028110: 7365 204e 6f6e 6529 0a20 2020 2020 2020  se None).       
-00028120: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
-00028130: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-00028140: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00028150: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
-00028160: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
-00028170: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-00028180: 6c66 2e74 6f74 616c 5f63 6f75 6e74 2069  lf.total_count i
-00028190: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000281a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000281b0: 546f 7461 6c43 6f75 6e74 275d 203d 2073  TotalCount'] = s
-000281c0: 656c 662e 746f 7461 6c5f 636f 756e 740a  elf.total_count.
-000281d0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000281e0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-000281f0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-00028200: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-00028210: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-00028220: 6469 6374 2829 0a20 2020 2020 2020 2073  dict().        s
-00028230: 656c 662e 6563 735f 7370 6563 7320 3d20  elf.ecs_specs = 
-00028240: 5b5d 0a20 2020 2020 2020 2069 6620 6d2e  [].        if m.
-00028250: 6765 7428 2745 6373 5370 6563 7327 2920  get('EcsSpecs') 
-00028260: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00028270: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
-00028280: 6e20 6d2e 6765 7428 2745 6373 5370 6563  n m.get('EcsSpec
-00028290: 7327 293a 0a20 2020 2020 2020 2020 2020  s'):.           
-000282a0: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
-000282b0: 3d20 4563 7353 7065 6328 290a 2020 2020  = EcsSpec().    
-000282c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000282d0: 2e65 6373 5f73 7065 6373 2e61 7070 656e  .ecs_specs.appen
-000282e0: 6428 7465 6d70 5f6d 6f64 656c 2e66 726f  d(temp_model.fro
-000282f0: 6d5f 6d61 7028 6b29 290a 2020 2020 2020  m_map(k)).      
-00028300: 2020 6966 206d 2e67 6574 2827 5265 7175    if m.get('Requ
-00028310: 6573 7449 6427 2920 6973 206e 6f74 204e  estId') is not N
-00028320: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00028330: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-00028340: 203d 206d 2e67 6574 2827 5265 7175 6573   = m.get('Reques
-00028350: 7449 6427 290a 2020 2020 2020 2020 6966  tId').        if
-00028360: 206d 2e67 6574 2827 546f 7461 6c43 6f75   m.get('TotalCou
-00028370: 6e74 2729 2069 7320 6e6f 7420 4e6f 6e65  nt') is not None
-00028380: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00028390: 6c66 2e74 6f74 616c 5f63 6f75 6e74 203d  lf.total_count =
-000283a0: 206d 2e67 6574 2827 546f 7461 6c43 6f75   m.get('TotalCou
-000283b0: 6e74 2729 0a20 2020 2020 2020 2072 6574  nt').        ret
-000283c0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-000283d0: 204c 6973 7445 6373 5370 6563 7352 6573   ListEcsSpecsRes
-000283e0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-000283f0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00028400: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00028410: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-00028420: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-00028430: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00028440: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-00028450: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-00028460: 2020 626f 6479 3a20 4c69 7374 4563 7353    body: ListEcsS
-00028470: 7065 6373 5265 7370 6f6e 7365 426f 6479  pecsResponseBody
-00028480: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-00028490: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-000284a0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-000284b0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-000284c0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-000284d0: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
-000284e0: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
-000284f0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00028500: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00028510: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-00028520: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
-00028530: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
-00028540: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-00028550: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-00028560: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
-00028570: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
-00028580: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-00028590: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-000285a0: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
-000285b0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-000285c0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-000285d0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-000285e0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-000285f0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-00028600: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-00028610: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-00028620: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-00028630: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00028640: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00028650: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-00028660: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-00028670: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-00028680: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-00028690: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000286a0: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-000286b0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-000286c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000286d0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-000286e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000286f0: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-00028700: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-00028710: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-00028720: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-00028730: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-00028740: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00028750: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-00028760: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-00028770: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00028780: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00028790: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-000287a0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-000287b0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-000287c0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000287d0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-000287e0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000287f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028800: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-00028810: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-00028820: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-00028830: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-00028840: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00028850: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-00028860: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-00028870: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-00028880: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-00028890: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000288a0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-000288b0: 5f6d 6f64 656c 203d 204c 6973 7445 6373  _model = ListEcs
-000288c0: 5370 6563 7352 6573 706f 6e73 6542 6f64  SpecsResponseBod
-000288d0: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-000288e0: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-000288f0: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-00028900: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-00028910: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-00028920: 0a63 6c61 7373 204c 6973 744a 6f62 7352  .class ListJobsR
-00028930: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-00028940: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00028950: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-00028960: 2c0a 2020 2020 2020 2020 6275 7369 6e65  ,.        busine
-00028970: 7373 5f75 7365 725f 6964 3a20 7374 7220  ss_user_id: str 
-00028980: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00028990: 6361 6c6c 6572 3a20 7374 7220 3d20 4e6f  caller: str = No
-000289a0: 6e65 2c0a 2020 2020 2020 2020 6469 7370  ne,.        disp
-000289b0: 6c61 795f 6e61 6d65 3a20 7374 7220 3d20  lay_name: str = 
-000289c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 656e  None,.        en
-000289d0: 645f 7469 6d65 3a20 7374 7220 3d20 4e6f  d_time: str = No
-000289e0: 6e65 2c0a 2020 2020 2020 2020 6672 6f6d  ne,.        from
-000289f0: 5f61 6c6c 5f77 6f72 6b73 7061 6365 733a  _all_workspaces:
-00028a00: 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020   bool = None,.  
-00028a10: 2020 2020 2020 6a6f 625f 6964 3a20 7374        job_id: st
-00028a20: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00028a30: 2020 6a6f 625f 7479 7065 3a20 7374 7220    job_type: str 
-00028a40: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00028a50: 6f72 6465 723a 2073 7472 203d 204e 6f6e  order: str = Non
-00028a60: 652c 0a20 2020 2020 2020 2070 6167 655f  e,.        page_
-00028a70: 6e75 6d62 6572 3a20 696e 7420 3d20 4e6f  number: int = No
-00028a80: 6e65 2c0a 2020 2020 2020 2020 7061 6765  ne,.        page
-00028a90: 5f73 697a 653a 2069 6e74 203d 204e 6f6e  _size: int = Non
-00028aa0: 652c 0a20 2020 2020 2020 2070 6970 656c  e,.        pipel
-00028ab0: 696e 655f 6964 3a20 7374 7220 3d20 4e6f  ine_id: str = No
-00028ac0: 6e65 2c0a 2020 2020 2020 2020 7265 736f  ne,.        reso
-00028ad0: 7572 6365 5f69 643a 2073 7472 203d 204e  urce_id: str = N
-00028ae0: 6f6e 652c 0a20 2020 2020 2020 2073 686f  one,.        sho
-00028af0: 775f 6f77 6e3a 2062 6f6f 6c20 3d20 4e6f  w_own: bool = No
-00028b00: 6e65 2c0a 2020 2020 2020 2020 736f 7274  ne,.        sort
-00028b10: 5f62 793a 2073 7472 203d 204e 6f6e 652c  _by: str = None,
-00028b20: 0a20 2020 2020 2020 2073 7461 7274 5f74  .        start_t
-00028b30: 696d 653a 2073 7472 203d 204e 6f6e 652c  ime: str = None,
-00028b40: 0a20 2020 2020 2020 2073 7461 7475 733a  .        status:
-00028b50: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00028b60: 2020 2020 2074 6167 733a 2044 6963 745b       tags: Dict[
-00028b70: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
-00028b80: 2c0a 2020 2020 2020 2020 776f 726b 7370  ,.        worksp
-00028b90: 6163 655f 6964 3a20 7374 7220 3d20 4e6f  ace_id: str = No
-00028ba0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-00028bb0: 2020 2073 656c 662e 6275 7369 6e65 7373     self.business
-00028bc0: 5f75 7365 725f 6964 203d 2062 7573 696e  _user_id = busin
-00028bd0: 6573 735f 7573 6572 5f69 640a 2020 2020  ess_user_id.    
-00028be0: 2020 2020 7365 6c66 2e63 616c 6c65 7220      self.caller 
-00028bf0: 3d20 6361 6c6c 6572 0a20 2020 2020 2020  = caller.       
-00028c00: 2073 656c 662e 6469 7370 6c61 795f 6e61   self.display_na
-00028c10: 6d65 203d 2064 6973 706c 6179 5f6e 616d  me = display_nam
-00028c20: 650a 2020 2020 2020 2020 7365 6c66 2e65  e.        self.e
-00028c30: 6e64 5f74 696d 6520 3d20 656e 645f 7469  nd_time = end_ti
-00028c40: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
-00028c50: 6672 6f6d 5f61 6c6c 5f77 6f72 6b73 7061  from_all_workspa
-00028c60: 6365 7320 3d20 6672 6f6d 5f61 6c6c 5f77  ces = from_all_w
-00028c70: 6f72 6b73 7061 6365 730a 2020 2020 2020  orkspaces.      
-00028c80: 2020 7365 6c66 2e6a 6f62 5f69 6420 3d20    self.job_id = 
-00028c90: 6a6f 625f 6964 0a20 2020 2020 2020 2073  job_id.        s
-00028ca0: 656c 662e 6a6f 625f 7479 7065 203d 206a  elf.job_type = j
-00028cb0: 6f62 5f74 7970 650a 2020 2020 2020 2020  ob_type.        
-00028cc0: 7365 6c66 2e6f 7264 6572 203d 206f 7264  self.order = ord
-00028cd0: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
-00028ce0: 7061 6765 5f6e 756d 6265 7220 3d20 7061  page_number = pa
-00028cf0: 6765 5f6e 756d 6265 720a 2020 2020 2020  ge_number.      
-00028d00: 2020 7365 6c66 2e70 6167 655f 7369 7a65    self.page_size
-00028d10: 203d 2070 6167 655f 7369 7a65 0a20 2020   = page_size.   
-00028d20: 2020 2020 2073 656c 662e 7069 7065 6c69       self.pipeli
-00028d30: 6e65 5f69 6420 3d20 7069 7065 6c69 6e65  ne_id = pipeline
-00028d40: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
-00028d50: 2e72 6573 6f75 7263 655f 6964 203d 2072  .resource_id = r
-00028d60: 6573 6f75 7263 655f 6964 0a20 2020 2020  esource_id.     
-00028d70: 2020 2073 656c 662e 7368 6f77 5f6f 776e     self.show_own
-00028d80: 203d 2073 686f 775f 6f77 6e0a 2020 2020   = show_own.    
-00028d90: 2020 2020 7365 6c66 2e73 6f72 745f 6279      self.sort_by
-00028da0: 203d 2073 6f72 745f 6279 0a20 2020 2020   = sort_by.     
-00028db0: 2020 2073 656c 662e 7374 6172 745f 7469     self.start_ti
-00028dc0: 6d65 203d 2073 7461 7274 5f74 696d 650a  me = start_time.
-00028dd0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00028de0: 7475 7320 3d20 7374 6174 7573 0a20 2020  tus = status.   
-00028df0: 2020 2020 2073 656c 662e 7461 6773 203d       self.tags =
-00028e00: 2074 6167 730a 2020 2020 2020 2020 7365   tags.        se
-00028e10: 6c66 2e77 6f72 6b73 7061 6365 5f69 6420  lf.workspace_id 
-00028e20: 3d20 776f 726b 7370 6163 655f 6964 0a0a  = workspace_id..
-00028e30: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00028e40: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00028e50: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-00028e60: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-00028e70: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-00028e80: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-00028e90: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-00028ea0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00028eb0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-00028ec0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00028ed0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-00028ee0: 2020 6966 2073 656c 662e 6275 7369 6e65    if self.busine
-00028ef0: 7373 5f75 7365 725f 6964 2069 7320 6e6f  ss_user_id is no
-00028f00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00028f10: 2020 2020 7265 7375 6c74 5b27 4275 7369      result['Busi
-00028f20: 6e65 7373 5573 6572 4964 275d 203d 2073  nessUserId'] = s
-00028f30: 656c 662e 6275 7369 6e65 7373 5f75 7365  elf.business_use
-00028f40: 725f 6964 0a20 2020 2020 2020 2069 6620  r_id.        if 
-00028f50: 7365 6c66 2e63 616c 6c65 7220 6973 206e  self.caller is n
-00028f60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00028f70: 2020 2020 2072 6573 756c 745b 2743 616c       result['Cal
-00028f80: 6c65 7227 5d20 3d20 7365 6c66 2e63 616c  ler'] = self.cal
-00028f90: 6c65 720a 2020 2020 2020 2020 6966 2073  ler.        if s
-00028fa0: 656c 662e 6469 7370 6c61 795f 6e61 6d65  elf.display_name
-00028fb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028fc0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00028fd0: 5b27 4469 7370 6c61 794e 616d 6527 5d20  ['DisplayName'] 
-00028fe0: 3d20 7365 6c66 2e64 6973 706c 6179 5f6e  = self.display_n
-00028ff0: 616d 650a 2020 2020 2020 2020 6966 2073  ame.        if s
-00029000: 656c 662e 656e 645f 7469 6d65 2069 7320  elf.end_time is 
-00029010: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029020: 2020 2020 2020 7265 7375 6c74 5b27 456e        result['En
-00029030: 6454 696d 6527 5d20 3d20 7365 6c66 2e65  dTime'] = self.e
-00029040: 6e64 5f74 696d 650a 2020 2020 2020 2020  nd_time.        
-00029050: 6966 2073 656c 662e 6672 6f6d 5f61 6c6c  if self.from_all
-00029060: 5f77 6f72 6b73 7061 6365 7320 6973 206e  _workspaces is n
-00029070: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00029080: 2020 2020 2072 6573 756c 745b 2746 726f       result['Fro
-00029090: 6d41 6c6c 576f 726b 7370 6163 6573 275d  mAllWorkspaces']
-000290a0: 203d 2073 656c 662e 6672 6f6d 5f61 6c6c   = self.from_all
-000290b0: 5f77 6f72 6b73 7061 6365 730a 2020 2020  _workspaces.    
-000290c0: 2020 2020 6966 2073 656c 662e 6a6f 625f      if self.job_
-000290d0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-000290e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000290f0: 6c74 5b27 4a6f 6249 6427 5d20 3d20 7365  lt['JobId'] = se
-00029100: 6c66 2e6a 6f62 5f69 640a 2020 2020 2020  lf.job_id.      
-00029110: 2020 6966 2073 656c 662e 6a6f 625f 7479    if self.job_ty
-00029120: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
-00029130: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00029140: 6c74 5b27 4a6f 6254 7970 6527 5d20 3d20  lt['JobType'] = 
-00029150: 7365 6c66 2e6a 6f62 5f74 7970 650a 2020  self.job_type.  
-00029160: 2020 2020 2020 6966 2073 656c 662e 6f72        if self.or
-00029170: 6465 7220 6973 206e 6f74 204e 6f6e 653a  der is not None:
-00029180: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00029190: 756c 745b 274f 7264 6572 275d 203d 2073  ult['Order'] = s
-000291a0: 656c 662e 6f72 6465 720a 2020 2020 2020  elf.order.      
-000291b0: 2020 6966 2073 656c 662e 7061 6765 5f6e    if self.page_n
-000291c0: 756d 6265 7220 6973 206e 6f74 204e 6f6e  umber is not Non
-000291d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000291e0: 6573 756c 745b 2750 6167 654e 756d 6265  esult['PageNumbe
-000291f0: 7227 5d20 3d20 7365 6c66 2e70 6167 655f  r'] = self.page_
-00029200: 6e75 6d62 6572 0a20 2020 2020 2020 2069  number.        i
-00029210: 6620 7365 6c66 2e70 6167 655f 7369 7a65  f self.page_size
-00029220: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00029230: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00029240: 5b27 5061 6765 5369 7a65 275d 203d 2073  ['PageSize'] = s
-00029250: 656c 662e 7061 6765 5f73 697a 650a 2020  elf.page_size.  
-00029260: 2020 2020 2020 6966 2073 656c 662e 7069        if self.pi
-00029270: 7065 6c69 6e65 5f69 6420 6973 206e 6f74  peline_id is not
-00029280: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00029290: 2020 2072 6573 756c 745b 2750 6970 656c     result['Pipel
-000292a0: 696e 6549 6427 5d20 3d20 7365 6c66 2e70  ineId'] = self.p
-000292b0: 6970 656c 696e 655f 6964 0a20 2020 2020  ipeline_id.     
-000292c0: 2020 2069 6620 7365 6c66 2e72 6573 6f75     if self.resou
-000292d0: 7263 655f 6964 2069 7320 6e6f 7420 4e6f  rce_id is not No
-000292e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000292f0: 7265 7375 6c74 5b27 5265 736f 7572 6365  result['Resource
-00029300: 4964 275d 203d 2073 656c 662e 7265 736f  Id'] = self.reso
-00029310: 7572 6365 5f69 640a 2020 2020 2020 2020  urce_id.        
-00029320: 6966 2073 656c 662e 7368 6f77 5f6f 776e  if self.show_own
-00029330: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00029340: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00029350: 5b27 5368 6f77 4f77 6e27 5d20 3d20 7365  ['ShowOwn'] = se
-00029360: 6c66 2e73 686f 775f 6f77 6e0a 2020 2020  lf.show_own.    
-00029370: 2020 2020 6966 2073 656c 662e 736f 7274      if self.sort
-00029380: 5f62 7920 6973 206e 6f74 204e 6f6e 653a  _by is not None:
-00029390: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000293a0: 756c 745b 2753 6f72 7442 7927 5d20 3d20  ult['SortBy'] = 
-000293b0: 7365 6c66 2e73 6f72 745f 6279 0a20 2020  self.sort_by.   
-000293c0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-000293d0: 7274 5f74 696d 6520 6973 206e 6f74 204e  rt_time is not N
-000293e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000293f0: 2072 6573 756c 745b 2753 7461 7274 5469   result['StartTi
-00029400: 6d65 275d 203d 2073 656c 662e 7374 6172  me'] = self.star
-00029410: 745f 7469 6d65 0a20 2020 2020 2020 2069  t_time.        i
-00029420: 6620 7365 6c66 2e73 7461 7475 7320 6973  f self.status is
-00029430: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00029440: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
-00029450: 7461 7475 7327 5d20 3d20 7365 6c66 2e73  tatus'] = self.s
-00029460: 7461 7475 730a 2020 2020 2020 2020 6966  tatus.        if
-00029470: 2073 656c 662e 7461 6773 2069 7320 6e6f   self.tags is no
-00029480: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00029490: 2020 2020 7265 7375 6c74 5b27 5461 6773      result['Tags
-000294a0: 275d 203d 2073 656c 662e 7461 6773 0a20  '] = self.tags. 
-000294b0: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
-000294c0: 6f72 6b73 7061 6365 5f69 6420 6973 206e  orkspace_id is n
-000294d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000294e0: 2020 2020 2072 6573 756c 745b 2757 6f72       result['Wor
-000294f0: 6b73 7061 6365 4964 275d 203d 2073 656c  kspaceId'] = sel
-00029500: 662e 776f 726b 7370 6163 655f 6964 0a20  f.workspace_id. 
-00029510: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00029520: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-00029530: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-00029540: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-00029550: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-00029560: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00029570: 206d 2e67 6574 2827 4275 7369 6e65 7373   m.get('Business
-00029580: 5573 6572 4964 2729 2069 7320 6e6f 7420  UserId') is not 
-00029590: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000295a0: 2020 7365 6c66 2e62 7573 696e 6573 735f    self.business_
-000295b0: 7573 6572 5f69 6420 3d20 6d2e 6765 7428  user_id = m.get(
-000295c0: 2742 7573 696e 6573 7355 7365 7249 6427  'BusinessUserId'
-000295d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-000295e0: 6574 2827 4361 6c6c 6572 2729 2069 7320  et('Caller') is 
-000295f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029600: 2020 2020 2020 7365 6c66 2e63 616c 6c65        self.calle
-00029610: 7220 3d20 6d2e 6765 7428 2743 616c 6c65  r = m.get('Calle
-00029620: 7227 290a 2020 2020 2020 2020 6966 206d  r').        if m
-00029630: 2e67 6574 2827 4469 7370 6c61 794e 616d  .get('DisplayNam
-00029640: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00029650: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00029660: 662e 6469 7370 6c61 795f 6e61 6d65 203d  f.display_name =
-00029670: 206d 2e67 6574 2827 4469 7370 6c61 794e   m.get('DisplayN
-00029680: 616d 6527 290a 2020 2020 2020 2020 6966  ame').        if
-00029690: 206d 2e67 6574 2827 456e 6454 696d 6527   m.get('EndTime'
-000296a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000296b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000296c0: 656e 645f 7469 6d65 203d 206d 2e67 6574  end_time = m.get
-000296d0: 2827 456e 6454 696d 6527 290a 2020 2020  ('EndTime').    
-000296e0: 2020 2020 6966 206d 2e67 6574 2827 4672      if m.get('Fr
-000296f0: 6f6d 416c 6c57 6f72 6b73 7061 6365 7327  omAllWorkspaces'
-00029700: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00029710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00029720: 6672 6f6d 5f61 6c6c 5f77 6f72 6b73 7061  from_all_workspa
-00029730: 6365 7320 3d20 6d2e 6765 7428 2746 726f  ces = m.get('Fro
-00029740: 6d41 6c6c 576f 726b 7370 6163 6573 2729  mAllWorkspaces')
-00029750: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00029760: 7428 274a 6f62 4964 2729 2069 7320 6e6f  t('JobId') is no
-00029770: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00029780: 2020 2020 7365 6c66 2e6a 6f62 5f69 6420      self.job_id 
-00029790: 3d20 6d2e 6765 7428 274a 6f62 4964 2729  = m.get('JobId')
-000297a0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-000297b0: 7428 274a 6f62 5479 7065 2729 2069 7320  t('JobType') is 
-000297c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000297d0: 2020 2020 2020 7365 6c66 2e6a 6f62 5f74        self.job_t
-000297e0: 7970 6520 3d20 6d2e 6765 7428 274a 6f62  ype = m.get('Job
-000297f0: 5479 7065 2729 0a20 2020 2020 2020 2069  Type').        i
-00029800: 6620 6d2e 6765 7428 274f 7264 6572 2729  f m.get('Order')
-00029810: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00029820: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
-00029830: 7264 6572 203d 206d 2e67 6574 2827 4f72  rder = m.get('Or
-00029840: 6465 7227 290a 2020 2020 2020 2020 6966  der').        if
-00029850: 206d 2e67 6574 2827 5061 6765 4e75 6d62   m.get('PageNumb
-00029860: 6572 2729 2069 7320 6e6f 7420 4e6f 6e65  er') is not None
-00029870: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00029880: 6c66 2e70 6167 655f 6e75 6d62 6572 203d  lf.page_number =
-00029890: 206d 2e67 6574 2827 5061 6765 4e75 6d62   m.get('PageNumb
-000298a0: 6572 2729 0a20 2020 2020 2020 2069 6620  er').        if 
-000298b0: 6d2e 6765 7428 2750 6167 6553 697a 6527  m.get('PageSize'
-000298c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-000298d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000298e0: 7061 6765 5f73 697a 6520 3d20 6d2e 6765  page_size = m.ge
-000298f0: 7428 2750 6167 6553 697a 6527 290a 2020  t('PageSize').  
-00029900: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00029910: 5069 7065 6c69 6e65 4964 2729 2069 7320  PipelineId') is 
-00029920: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029930: 2020 2020 2020 7365 6c66 2e70 6970 656c        self.pipel
-00029940: 696e 655f 6964 203d 206d 2e67 6574 2827  ine_id = m.get('
-00029950: 5069 7065 6c69 6e65 4964 2729 0a20 2020  PipelineId').   
-00029960: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-00029970: 6573 6f75 7263 6549 6427 2920 6973 206e  esourceId') is n
-00029980: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00029990: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
-000299a0: 6365 5f69 6420 3d20 6d2e 6765 7428 2752  ce_id = m.get('R
-000299b0: 6573 6f75 7263 6549 6427 290a 2020 2020  esourceId').    
-000299c0: 2020 2020 6966 206d 2e67 6574 2827 5368      if m.get('Sh
-000299d0: 6f77 4f77 6e27 2920 6973 206e 6f74 204e  owOwn') is not N
-000299e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000299f0: 2073 656c 662e 7368 6f77 5f6f 776e 203d   self.show_own =
-00029a00: 206d 2e67 6574 2827 5368 6f77 4f77 6e27   m.get('ShowOwn'
-00029a10: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00029a20: 6574 2827 536f 7274 4279 2729 2069 7320  et('SortBy') is 
-00029a30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029a40: 2020 2020 2020 7365 6c66 2e73 6f72 745f        self.sort_
-00029a50: 6279 203d 206d 2e67 6574 2827 536f 7274  by = m.get('Sort
-00029a60: 4279 2729 0a20 2020 2020 2020 2069 6620  By').        if 
-00029a70: 6d2e 6765 7428 2753 7461 7274 5469 6d65  m.get('StartTime
-00029a80: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00029a90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00029aa0: 2e73 7461 7274 5f74 696d 6520 3d20 6d2e  .start_time = m.
-00029ab0: 6765 7428 2753 7461 7274 5469 6d65 2729  get('StartTime')
-00029ac0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00029ad0: 7428 2753 7461 7475 7327 2920 6973 206e  t('Status') is n
-00029ae0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00029af0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00029b00: 203d 206d 2e67 6574 2827 5374 6174 7573   = m.get('Status
-00029b10: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00029b20: 6765 7428 2754 6167 7327 2920 6973 206e  get('Tags') is n
-00029b30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00029b40: 2020 2020 2073 656c 662e 7461 6773 203d       self.tags =
-00029b50: 206d 2e67 6574 2827 5461 6773 2729 0a20   m.get('Tags'). 
-00029b60: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00029b70: 2757 6f72 6b73 7061 6365 4964 2729 2069  'WorkspaceId') i
-00029b80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00029b90: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
-00029ba0: 6b73 7061 6365 5f69 6420 3d20 6d2e 6765  kspace_id = m.ge
-00029bb0: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
-00029bc0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00029bd0: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
-00029be0: 744a 6f62 7353 6872 696e 6b52 6571 7565  tJobsShrinkReque
-00029bf0: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
-00029c00: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00029c10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00029c20: 2020 2020 2020 6275 7369 6e65 7373 5f75        business_u
-00029c30: 7365 725f 6964 3a20 7374 7220 3d20 4e6f  ser_id: str = No
-00029c40: 6e65 2c0a 2020 2020 2020 2020 6361 6c6c  ne,.        call
-00029c50: 6572 3a20 7374 7220 3d20 4e6f 6e65 2c0a  er: str = None,.
-00029c60: 2020 2020 2020 2020 6469 7370 6c61 795f          display_
-00029c70: 6e61 6d65 3a20 7374 7220 3d20 4e6f 6e65  name: str = None
-00029c80: 2c0a 2020 2020 2020 2020 656e 645f 7469  ,.        end_ti
-00029c90: 6d65 3a20 7374 7220 3d20 4e6f 6e65 2c0a  me: str = None,.
-00029ca0: 2020 2020 2020 2020 6672 6f6d 5f61 6c6c          from_all
-00029cb0: 5f77 6f72 6b73 7061 6365 733a 2062 6f6f  _workspaces: boo
-00029cc0: 6c20 3d20 4e6f 6e65 2c0a 2020 2020 2020  l = None,.      
-00029cd0: 2020 6a6f 625f 6964 3a20 7374 7220 3d20    job_id: str = 
-00029ce0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6a6f  None,.        jo
-00029cf0: 625f 7479 7065 3a20 7374 7220 3d20 4e6f  b_type: str = No
-00029d00: 6e65 2c0a 2020 2020 2020 2020 6f72 6465  ne,.        orde
-00029d10: 723a 2073 7472 203d 204e 6f6e 652c 0a20  r: str = None,. 
-00029d20: 2020 2020 2020 2070 6167 655f 6e75 6d62         page_numb
-00029d30: 6572 3a20 696e 7420 3d20 4e6f 6e65 2c0a  er: int = None,.
-00029d40: 2020 2020 2020 2020 7061 6765 5f73 697a          page_siz
-00029d50: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
-00029d60: 2020 2020 2020 2070 6970 656c 696e 655f         pipeline_
-00029d70: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-00029d80: 2020 2020 2020 2020 7265 736f 7572 6365          resource
-00029d90: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-00029da0: 0a20 2020 2020 2020 2073 686f 775f 6f77  .        show_ow
-00029db0: 6e3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  n: bool = None,.
-00029dc0: 2020 2020 2020 2020 736f 7274 5f62 793a          sort_by:
-00029dd0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00029de0: 2020 2020 2073 7461 7274 5f74 696d 653a       start_time:
-00029df0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00029e00: 2020 2020 2073 7461 7475 733a 2073 7472       status: str
-00029e10: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00029e20: 2074 6167 735f 7368 7269 6e6b 3a20 7374   tags_shrink: st
-00029e30: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00029e40: 2020 776f 726b 7370 6163 655f 6964 3a20    workspace_id: 
-00029e50: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-00029e60: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00029e70: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
-00029e80: 203d 2062 7573 696e 6573 735f 7573 6572   = business_user
-00029e90: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
-00029ea0: 2e63 616c 6c65 7220 3d20 6361 6c6c 6572  .caller = caller
-00029eb0: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
-00029ec0: 7370 6c61 795f 6e61 6d65 203d 2064 6973  splay_name = dis
-00029ed0: 706c 6179 5f6e 616d 650a 2020 2020 2020  play_name.      
-00029ee0: 2020 7365 6c66 2e65 6e64 5f74 696d 6520    self.end_time 
-00029ef0: 3d20 656e 645f 7469 6d65 0a20 2020 2020  = end_time.     
-00029f00: 2020 2073 656c 662e 6672 6f6d 5f61 6c6c     self.from_all
-00029f10: 5f77 6f72 6b73 7061 6365 7320 3d20 6672  _workspaces = fr
-00029f20: 6f6d 5f61 6c6c 5f77 6f72 6b73 7061 6365  om_all_workspace
-00029f30: 730a 2020 2020 2020 2020 7365 6c66 2e6a  s.        self.j
-00029f40: 6f62 5f69 6420 3d20 6a6f 625f 6964 0a20  ob_id = job_id. 
-00029f50: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
-00029f60: 7479 7065 203d 206a 6f62 5f74 7970 650a  type = job_type.
-00029f70: 2020 2020 2020 2020 7365 6c66 2e6f 7264          self.ord
-00029f80: 6572 203d 206f 7264 6572 0a20 2020 2020  er = order.     
-00029f90: 2020 2073 656c 662e 7061 6765 5f6e 756d     self.page_num
-00029fa0: 6265 7220 3d20 7061 6765 5f6e 756d 6265  ber = page_numbe
-00029fb0: 720a 2020 2020 2020 2020 7365 6c66 2e70  r.        self.p
-00029fc0: 6167 655f 7369 7a65 203d 2070 6167 655f  age_size = page_
-00029fd0: 7369 7a65 0a20 2020 2020 2020 2073 656c  size.        sel
-00029fe0: 662e 7069 7065 6c69 6e65 5f69 6420 3d20  f.pipeline_id = 
-00029ff0: 7069 7065 6c69 6e65 5f69 640a 2020 2020  pipeline_id.    
-0002a000: 2020 2020 7365 6c66 2e72 6573 6f75 7263      self.resourc
-0002a010: 655f 6964 203d 2072 6573 6f75 7263 655f  e_id = resource_
-0002a020: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
-0002a030: 7368 6f77 5f6f 776e 203d 2073 686f 775f  show_own = show_
-0002a040: 6f77 6e0a 2020 2020 2020 2020 7365 6c66  own.        self
-0002a050: 2e73 6f72 745f 6279 203d 2073 6f72 745f  .sort_by = sort_
-0002a060: 6279 0a20 2020 2020 2020 2073 656c 662e  by.        self.
-0002a070: 7374 6172 745f 7469 6d65 203d 2073 7461  start_time = sta
-0002a080: 7274 5f74 696d 650a 2020 2020 2020 2020  rt_time.        
-0002a090: 7365 6c66 2e73 7461 7475 7320 3d20 7374  self.status = st
-0002a0a0: 6174 7573 0a20 2020 2020 2020 2073 656c  atus.        sel
-0002a0b0: 662e 7461 6773 5f73 6872 696e 6b20 3d20  f.tags_shrink = 
-0002a0c0: 7461 6773 5f73 6872 696e 6b0a 2020 2020  tags_shrink.    
-0002a0d0: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
-0002a0e0: 6365 5f69 6420 3d20 776f 726b 7370 6163  ce_id = workspac
-0002a0f0: 655f 6964 0a0a 2020 2020 6465 6620 7661  e_id..    def va
-0002a100: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-0002a110: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-0002a120: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-0002a130: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-0002a140: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-0002a150: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-0002a160: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-0002a170: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0002a180: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-0002a190: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-0002a1a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002a1b0: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
-0002a1c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002a1d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002a1e0: 5b27 4275 7369 6e65 7373 5573 6572 4964  ['BusinessUserId
-0002a1f0: 275d 203d 2073 656c 662e 6275 7369 6e65  '] = self.busine
-0002a200: 7373 5f75 7365 725f 6964 0a20 2020 2020  ss_user_id.     
-0002a210: 2020 2069 6620 7365 6c66 2e63 616c 6c65     if self.calle
-0002a220: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-0002a230: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002a240: 745b 2743 616c 6c65 7227 5d20 3d20 7365  t['Caller'] = se
-0002a250: 6c66 2e63 616c 6c65 720a 2020 2020 2020  lf.caller.      
-0002a260: 2020 6966 2073 656c 662e 6469 7370 6c61    if self.displa
-0002a270: 795f 6e61 6d65 2069 7320 6e6f 7420 4e6f  y_name is not No
-0002a280: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002a290: 7265 7375 6c74 5b27 4469 7370 6c61 794e  result['DisplayN
-0002a2a0: 616d 6527 5d20 3d20 7365 6c66 2e64 6973  ame'] = self.dis
-0002a2b0: 706c 6179 5f6e 616d 650a 2020 2020 2020  play_name.      
-0002a2c0: 2020 6966 2073 656c 662e 656e 645f 7469    if self.end_ti
-0002a2d0: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
-0002a2e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002a2f0: 6c74 5b27 456e 6454 696d 6527 5d20 3d20  lt['EndTime'] = 
-0002a300: 7365 6c66 2e65 6e64 5f74 696d 650a 2020  self.end_time.  
-0002a310: 2020 2020 2020 6966 2073 656c 662e 6672        if self.fr
-0002a320: 6f6d 5f61 6c6c 5f77 6f72 6b73 7061 6365  om_all_workspace
-0002a330: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-0002a340: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002a350: 745b 2746 726f 6d41 6c6c 576f 726b 7370  t['FromAllWorksp
-0002a360: 6163 6573 275d 203d 2073 656c 662e 6672  aces'] = self.fr
-0002a370: 6f6d 5f61 6c6c 5f77 6f72 6b73 7061 6365  om_all_workspace
-0002a380: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-0002a390: 662e 6a6f 625f 6964 2069 7320 6e6f 7420  f.job_id is not 
-0002a3a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002a3b0: 2020 7265 7375 6c74 5b27 4a6f 6249 6427    result['JobId'
-0002a3c0: 5d20 3d20 7365 6c66 2e6a 6f62 5f69 640a  ] = self.job_id.
-0002a3d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002a3e0: 6a6f 625f 7479 7065 2069 7320 6e6f 7420  job_type is not 
-0002a3f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002a400: 2020 7265 7375 6c74 5b27 4a6f 6254 7970    result['JobTyp
-0002a410: 6527 5d20 3d20 7365 6c66 2e6a 6f62 5f74  e'] = self.job_t
-0002a420: 7970 650a 2020 2020 2020 2020 6966 2073  ype.        if s
-0002a430: 656c 662e 6f72 6465 7220 6973 206e 6f74  elf.order is not
-0002a440: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002a450: 2020 2072 6573 756c 745b 274f 7264 6572     result['Order
-0002a460: 275d 203d 2073 656c 662e 6f72 6465 720a  '] = self.order.
-0002a470: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002a480: 7061 6765 5f6e 756d 6265 7220 6973 206e  page_number is n
-0002a490: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002a4a0: 2020 2020 2072 6573 756c 745b 2750 6167       result['Pag
-0002a4b0: 654e 756d 6265 7227 5d20 3d20 7365 6c66  eNumber'] = self
-0002a4c0: 2e70 6167 655f 6e75 6d62 6572 0a20 2020  .page_number.   
-0002a4d0: 2020 2020 2069 6620 7365 6c66 2e70 6167       if self.pag
-0002a4e0: 655f 7369 7a65 2069 7320 6e6f 7420 4e6f  e_size is not No
-0002a4f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002a500: 7265 7375 6c74 5b27 5061 6765 5369 7a65  result['PageSize
-0002a510: 275d 203d 2073 656c 662e 7061 6765 5f73  '] = self.page_s
-0002a520: 697a 650a 2020 2020 2020 2020 6966 2073  ize.        if s
-0002a530: 656c 662e 7069 7065 6c69 6e65 5f69 6420  elf.pipeline_id 
-0002a540: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002a550: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002a560: 2750 6970 656c 696e 6549 6427 5d20 3d20  'PipelineId'] = 
-0002a570: 7365 6c66 2e70 6970 656c 696e 655f 6964  self.pipeline_id
-0002a580: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002a590: 2e72 6573 6f75 7263 655f 6964 2069 7320  .resource_id is 
-0002a5a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002a5b0: 2020 2020 2020 7265 7375 6c74 5b27 5265        result['Re
-0002a5c0: 736f 7572 6365 4964 275d 203d 2073 656c  sourceId'] = sel
-0002a5d0: 662e 7265 736f 7572 6365 5f69 640a 2020  f.resource_id.  
-0002a5e0: 2020 2020 2020 6966 2073 656c 662e 7368        if self.sh
-0002a5f0: 6f77 5f6f 776e 2069 7320 6e6f 7420 4e6f  ow_own is not No
-0002a600: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002a610: 7265 7375 6c74 5b27 5368 6f77 4f77 6e27  result['ShowOwn'
-0002a620: 5d20 3d20 7365 6c66 2e73 686f 775f 6f77  ] = self.show_ow
-0002a630: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-0002a640: 662e 736f 7274 5f62 7920 6973 206e 6f74  f.sort_by is not
-0002a650: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002a660: 2020 2072 6573 756c 745b 2753 6f72 7442     result['SortB
-0002a670: 7927 5d20 3d20 7365 6c66 2e73 6f72 745f  y'] = self.sort_
-0002a680: 6279 0a20 2020 2020 2020 2069 6620 7365  by.        if se
-0002a690: 6c66 2e73 7461 7274 5f74 696d 6520 6973  lf.start_time is
-0002a6a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002a6b0: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
-0002a6c0: 7461 7274 5469 6d65 275d 203d 2073 656c  tartTime'] = sel
-0002a6d0: 662e 7374 6172 745f 7469 6d65 0a20 2020  f.start_time.   
-0002a6e0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-0002a6f0: 7475 7320 6973 206e 6f74 204e 6f6e 653a  tus is not None:
-0002a700: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002a710: 756c 745b 2753 7461 7475 7327 5d20 3d20  ult['Status'] = 
-0002a720: 7365 6c66 2e73 7461 7475 730a 2020 2020  self.status.    
-0002a730: 2020 2020 6966 2073 656c 662e 7461 6773      if self.tags
-0002a740: 5f73 6872 696e 6b20 6973 206e 6f74 204e  _shrink is not N
-0002a750: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002a760: 2072 6573 756c 745b 2754 6167 7327 5d20   result['Tags'] 
-0002a770: 3d20 7365 6c66 2e74 6167 735f 7368 7269  = self.tags_shri
-0002a780: 6e6b 0a20 2020 2020 2020 2069 6620 7365  nk.        if se
-0002a790: 6c66 2e77 6f72 6b73 7061 6365 5f69 6420  lf.workspace_id 
-0002a7a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002a7b0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002a7c0: 2757 6f72 6b73 7061 6365 4964 275d 203d  'WorkspaceId'] =
-0002a7d0: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
-0002a7e0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-0002a7f0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0002a800: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0002a810: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-0002a820: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-0002a830: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-0002a840: 2020 6966 206d 2e67 6574 2827 4275 7369    if m.get('Busi
-0002a850: 6e65 7373 5573 6572 4964 2729 2069 7320  nessUserId') is 
-0002a860: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002a870: 2020 2020 2020 7365 6c66 2e62 7573 696e        self.busin
-0002a880: 6573 735f 7573 6572 5f69 6420 3d20 6d2e  ess_user_id = m.
-0002a890: 6765 7428 2742 7573 696e 6573 7355 7365  get('BusinessUse
-0002a8a0: 7249 6427 290a 2020 2020 2020 2020 6966  rId').        if
-0002a8b0: 206d 2e67 6574 2827 4361 6c6c 6572 2729   m.get('Caller')
-0002a8c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002a8d0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0002a8e0: 616c 6c65 7220 3d20 6d2e 6765 7428 2743  aller = m.get('C
-0002a8f0: 616c 6c65 7227 290a 2020 2020 2020 2020  aller').        
-0002a900: 6966 206d 2e67 6574 2827 4469 7370 6c61  if m.get('Displa
-0002a910: 794e 616d 6527 2920 6973 206e 6f74 204e  yName') is not N
-0002a920: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002a930: 2073 656c 662e 6469 7370 6c61 795f 6e61   self.display_na
-0002a940: 6d65 203d 206d 2e67 6574 2827 4469 7370  me = m.get('Disp
-0002a950: 6c61 794e 616d 6527 290a 2020 2020 2020  layName').      
-0002a960: 2020 6966 206d 2e67 6574 2827 456e 6454    if m.get('EndT
-0002a970: 696d 6527 2920 6973 206e 6f74 204e 6f6e  ime') is not Non
-0002a980: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002a990: 656c 662e 656e 645f 7469 6d65 203d 206d  elf.end_time = m
-0002a9a0: 2e67 6574 2827 456e 6454 696d 6527 290a  .get('EndTime').
-0002a9b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002a9c0: 2827 4672 6f6d 416c 6c57 6f72 6b73 7061  ('FromAllWorkspa
-0002a9d0: 6365 7327 2920 6973 206e 6f74 204e 6f6e  ces') is not Non
-0002a9e0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002a9f0: 656c 662e 6672 6f6d 5f61 6c6c 5f77 6f72  elf.from_all_wor
-0002aa00: 6b73 7061 6365 7320 3d20 6d2e 6765 7428  kspaces = m.get(
-0002aa10: 2746 726f 6d41 6c6c 576f 726b 7370 6163  'FromAllWorkspac
-0002aa20: 6573 2729 0a20 2020 2020 2020 2069 6620  es').        if 
-0002aa30: 6d2e 6765 7428 274a 6f62 4964 2729 2069  m.get('JobId') i
-0002aa40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002aa50: 2020 2020 2020 2020 7365 6c66 2e6a 6f62          self.job
-0002aa60: 5f69 6420 3d20 6d2e 6765 7428 274a 6f62  _id = m.get('Job
-0002aa70: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-0002aa80: 6d2e 6765 7428 274a 6f62 5479 7065 2729  m.get('JobType')
-0002aa90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002aaa0: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
-0002aab0: 6f62 5f74 7970 6520 3d20 6d2e 6765 7428  ob_type = m.get(
-0002aac0: 274a 6f62 5479 7065 2729 0a20 2020 2020  'JobType').     
-0002aad0: 2020 2069 6620 6d2e 6765 7428 274f 7264     if m.get('Ord
-0002aae0: 6572 2729 2069 7320 6e6f 7420 4e6f 6e65  er') is not None
-0002aaf0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002ab00: 6c66 2e6f 7264 6572 203d 206d 2e67 6574  lf.order = m.get
-0002ab10: 2827 4f72 6465 7227 290a 2020 2020 2020  ('Order').      
-0002ab20: 2020 6966 206d 2e67 6574 2827 5061 6765    if m.get('Page
-0002ab30: 4e75 6d62 6572 2729 2069 7320 6e6f 7420  Number') is not 
-0002ab40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002ab50: 2020 7365 6c66 2e70 6167 655f 6e75 6d62    self.page_numb
-0002ab60: 6572 203d 206d 2e67 6574 2827 5061 6765  er = m.get('Page
-0002ab70: 4e75 6d62 6572 2729 0a20 2020 2020 2020  Number').       
-0002ab80: 2069 6620 6d2e 6765 7428 2750 6167 6553   if m.get('PageS
-0002ab90: 697a 6527 2920 6973 206e 6f74 204e 6f6e  ize') is not Non
-0002aba0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002abb0: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
-0002abc0: 6d2e 6765 7428 2750 6167 6553 697a 6527  m.get('PageSize'
-0002abd0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002abe0: 6574 2827 5069 7065 6c69 6e65 4964 2729  et('PipelineId')
-0002abf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002ac00: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0002ac10: 6970 656c 696e 655f 6964 203d 206d 2e67  ipeline_id = m.g
-0002ac20: 6574 2827 5069 7065 6c69 6e65 4964 2729  et('PipelineId')
-0002ac30: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002ac40: 7428 2752 6573 6f75 7263 6549 6427 2920  t('ResourceId') 
-0002ac50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002ac60: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0002ac70: 736f 7572 6365 5f69 6420 3d20 6d2e 6765  source_id = m.ge
-0002ac80: 7428 2752 6573 6f75 7263 6549 6427 290a  t('ResourceId').
-0002ac90: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002aca0: 2827 5368 6f77 4f77 6e27 2920 6973 206e  ('ShowOwn') is n
-0002acb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002acc0: 2020 2020 2073 656c 662e 7368 6f77 5f6f       self.show_o
-0002acd0: 776e 203d 206d 2e67 6574 2827 5368 6f77  wn = m.get('Show
-0002ace0: 4f77 6e27 290a 2020 2020 2020 2020 6966  Own').        if
-0002acf0: 206d 2e67 6574 2827 536f 7274 4279 2729   m.get('SortBy')
-0002ad00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002ad10: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0002ad20: 6f72 745f 6279 203d 206d 2e67 6574 2827  ort_by = m.get('
-0002ad30: 536f 7274 4279 2729 0a20 2020 2020 2020  SortBy').       
-0002ad40: 2069 6620 6d2e 6765 7428 2753 7461 7274   if m.get('Start
-0002ad50: 5469 6d65 2729 2069 7320 6e6f 7420 4e6f  Time') is not No
-0002ad60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002ad70: 7365 6c66 2e73 7461 7274 5f74 696d 6520  self.start_time 
-0002ad80: 3d20 6d2e 6765 7428 2753 7461 7274 5469  = m.get('StartTi
-0002ad90: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
-0002ada0: 6d2e 6765 7428 2753 7461 7475 7327 2920  m.get('Status') 
-0002adb0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002adc0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-0002add0: 6174 7573 203d 206d 2e67 6574 2827 5374  atus = m.get('St
-0002ade0: 6174 7573 2729 0a20 2020 2020 2020 2069  atus').        i
-0002adf0: 6620 6d2e 6765 7428 2754 6167 7327 2920  f m.get('Tags') 
-0002ae00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002ae10: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
-0002ae20: 6773 5f73 6872 696e 6b20 3d20 6d2e 6765  gs_shrink = m.ge
-0002ae30: 7428 2754 6167 7327 290a 2020 2020 2020  t('Tags').      
-0002ae40: 2020 6966 206d 2e67 6574 2827 576f 726b    if m.get('Work
-0002ae50: 7370 6163 6549 6427 2920 6973 206e 6f74  spaceId') is not
-0002ae60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002ae70: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
-0002ae80: 655f 6964 203d 206d 2e67 6574 2827 576f  e_id = m.get('Wo
-0002ae90: 726b 7370 6163 6549 6427 290a 2020 2020  rkspaceId').    
-0002aea0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0002aeb0: 0a0a 636c 6173 7320 4c69 7374 4a6f 6273  ..class ListJobs
-0002aec0: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
-0002aed0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0002aee0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0002aef0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0002af00: 6a6f 6273 3a20 4c69 7374 5b4a 6f62 4974  jobs: List[JobIt
-0002af10: 656d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  em] = None,.    
-0002af20: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
-0002af30: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
-0002af40: 2020 2020 746f 7461 6c5f 636f 756e 743a      total_count:
-0002af50: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-0002af60: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-0002af70: 2e6a 6f62 7320 3d20 6a6f 6273 0a20 2020  .jobs = jobs.   
-0002af80: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-0002af90: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
-0002afa0: 640a 2020 2020 2020 2020 7365 6c66 2e74  d.        self.t
-0002afb0: 6f74 616c 5f63 6f75 6e74 203d 2074 6f74  otal_count = tot
-0002afc0: 616c 5f63 6f75 6e74 0a0a 2020 2020 6465  al_count..    de
-0002afd0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0002afe0: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-0002aff0: 662e 6a6f 6273 3a0a 2020 2020 2020 2020  f.jobs:.        
-0002b000: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
-0002b010: 662e 6a6f 6273 3a0a 2020 2020 2020 2020  f.jobs:.        
-0002b020: 2020 2020 2020 2020 6966 206b 3a0a 2020          if k:.  
-0002b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002b040: 2020 6b2e 7661 6c69 6461 7465 2829 0a0a    k.validate()..
-0002b050: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0002b060: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0002b070: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-0002b080: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-0002b090: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-0002b0a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002b0b0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-0002b0c0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-0002b0d0: 7428 290a 2020 2020 2020 2020 7265 7375  t().        resu
-0002b0e0: 6c74 5b27 4a6f 6273 275d 203d 205b 5d0a  lt['Jobs'] = [].
-0002b0f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002b100: 6a6f 6273 2069 7320 6e6f 7420 4e6f 6e65  jobs is not None
-0002b110: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0002b120: 7220 6b20 696e 2073 656c 662e 6a6f 6273  r k in self.jobs
-0002b130: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002b140: 2020 7265 7375 6c74 5b27 4a6f 6273 275d    result['Jobs']
-0002b150: 2e61 7070 656e 6428 6b2e 746f 5f6d 6170  .append(k.to_map
-0002b160: 2829 2069 6620 6b20 656c 7365 204e 6f6e  () if k else Non
-0002b170: 6529 0a20 2020 2020 2020 2069 6620 7365  e).        if se
-0002b180: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
-0002b190: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002b1a0: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-0002b1b0: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
-0002b1c0: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
-0002b1d0: 2020 2020 2069 6620 7365 6c66 2e74 6f74       if self.tot
-0002b1e0: 616c 5f63 6f75 6e74 2069 7320 6e6f 7420  al_count is not 
-0002b1f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002b200: 2020 7265 7375 6c74 5b27 546f 7461 6c43    result['TotalC
-0002b210: 6f75 6e74 275d 203d 2073 656c 662e 746f  ount'] = self.to
-0002b220: 7461 6c5f 636f 756e 740a 2020 2020 2020  tal_count.      
-0002b230: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0002b240: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0002b250: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-0002b260: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-0002b270: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-0002b280: 0a20 2020 2020 2020 2073 656c 662e 6a6f  .        self.jo
-0002b290: 6273 203d 205b 5d0a 2020 2020 2020 2020  bs = [].        
-0002b2a0: 6966 206d 2e67 6574 2827 4a6f 6273 2729  if m.get('Jobs')
-0002b2b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002b2c0: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
-0002b2d0: 696e 206d 2e67 6574 2827 4a6f 6273 2729  in m.get('Jobs')
-0002b2e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002b2f0: 2020 7465 6d70 5f6d 6f64 656c 203d 204a    temp_model = J
-0002b300: 6f62 4974 656d 2829 0a20 2020 2020 2020  obItem().       
-0002b310: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
-0002b320: 6273 2e61 7070 656e 6428 7465 6d70 5f6d  bs.append(temp_m
-0002b330: 6f64 656c 2e66 726f 6d5f 6d61 7028 6b29  odel.from_map(k)
-0002b340: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002b350: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
-0002b360: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002b370: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0002b380: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
-0002b390: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
-0002b3a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002b3b0: 546f 7461 6c43 6f75 6e74 2729 2069 7320  TotalCount') is 
-0002b3c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002b3d0: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
-0002b3e0: 5f63 6f75 6e74 203d 206d 2e67 6574 2827  _count = m.get('
-0002b3f0: 546f 7461 6c43 6f75 6e74 2729 0a20 2020  TotalCount').   
-0002b400: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0002b410: 0a0a 0a63 6c61 7373 204c 6973 744a 6f62  ...class ListJob
-0002b420: 7352 6573 706f 6e73 6528 5465 614d 6f64  sResponse(TeaMod
-0002b430: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-0002b440: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0002b450: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
-0002b460: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
-0002b470: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0002b480: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
-0002b490: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-0002b4a0: 2020 2020 2020 626f 6479 3a20 4c69 7374        body: List
-0002b4b0: 4a6f 6273 5265 7370 6f6e 7365 426f 6479  JobsResponseBody
-0002b4c0: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-0002b4d0: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0002b4e0: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
-0002b4f0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0002b500: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
-0002b510: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
-0002b520: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
-0002b530: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0002b540: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002b550: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-0002b560: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
-0002b570: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
-0002b580: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-0002b590: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-0002b5a0: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
-0002b5b0: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
-0002b5c0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-0002b5d0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-0002b5e0: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
-0002b5f0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0002b600: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
-0002b610: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
-0002b620: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-0002b630: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0002b640: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0002b650: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
-0002b660: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0002b670: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002b680: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0002b690: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0002b6a0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0002b6b0: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-0002b6c0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-0002b6d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002b6e0: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-0002b6f0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-0002b700: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002b710: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-0002b720: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002b730: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-0002b740: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-0002b750: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-0002b760: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0002b770: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-0002b780: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002b790: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-0002b7a0: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-0002b7b0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002b7c0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0002b7d0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-0002b7e0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-0002b7f0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0002b800: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0002b810: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-0002b820: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002b830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002b840: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
-0002b850: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-0002b860: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
-0002b870: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
-0002b880: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002b890: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-0002b8a0: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
-0002b8b0: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
-0002b8c0: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
-0002b8d0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002b8e0: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0002b8f0: 5f6d 6f64 656c 203d 204c 6973 744a 6f62  _model = ListJob
-0002b900: 7352 6573 706f 6e73 6542 6f64 7928 290a  sResponseBody().
-0002b910: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002b920: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-0002b930: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-0002b940: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-0002b950: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-0002b960: 7373 204c 6973 7454 656e 736f 7262 6f61  ss ListTensorboa
-0002b970: 7264 7352 6571 7565 7374 2854 6561 4d6f  rdsRequest(TeaMo
-0002b980: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0002b990: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0002b9a0: 7365 6c66 2c0a 2020 2020 2020 2020 6469  self,.        di
-0002b9b0: 7370 6c61 795f 6e61 6d65 3a20 7374 7220  splay_name: str 
-0002b9c0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0002b9d0: 656e 645f 7469 6d65 3a20 7374 7220 3d20  end_time: str = 
-0002b9e0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6a6f  None,.        jo
-0002b9f0: 625f 6964 3a20 7374 7220 3d20 4e6f 6e65  b_id: str = None
-0002ba00: 2c0a 2020 2020 2020 2020 6f72 6465 723a  ,.        order:
-0002ba10: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0002ba20: 2020 2020 2070 6167 655f 6e75 6d62 6572       page_number
-0002ba30: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-0002ba40: 2020 2020 2020 7061 6765 5f73 697a 653a        page_size:
-0002ba50: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-0002ba60: 2020 2020 2073 6f72 745f 6279 3a20 7374       sort_by: st
-0002ba70: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0002ba80: 2020 736f 7572 6365 5f69 643a 2073 7472    source_id: str
-0002ba90: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0002baa0: 2073 6f75 7263 655f 7479 7065 3a20 7374   source_type: st
-0002bab0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0002bac0: 2020 7374 6172 745f 7469 6d65 3a20 7374    start_time: st
-0002bad0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0002bae0: 2020 7374 6174 7573 3a20 7374 7220 3d20    status: str = 
-0002baf0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7465  None,.        te
-0002bb00: 6e73 6f72 626f 6172 645f 6964 3a20 7374  nsorboard_id: st
-0002bb10: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-0002bb20: 2020 7665 7262 6f73 653a 2062 6f6f 6c20    verbose: bool 
-0002bb30: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0002bb40: 776f 726b 7370 6163 655f 6964 3a20 7374  workspace_id: st
-0002bb50: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
-0002bb60: 0a20 2020 2020 2020 2073 656c 662e 6469  .        self.di
-0002bb70: 7370 6c61 795f 6e61 6d65 203d 2064 6973  splay_name = dis
-0002bb80: 706c 6179 5f6e 616d 650a 2020 2020 2020  play_name.      
-0002bb90: 2020 7365 6c66 2e65 6e64 5f74 696d 6520    self.end_time 
-0002bba0: 3d20 656e 645f 7469 6d65 0a20 2020 2020  = end_time.     
-0002bbb0: 2020 2073 656c 662e 6a6f 625f 6964 203d     self.job_id =
-0002bbc0: 206a 6f62 5f69 640a 2020 2020 2020 2020   job_id.        
-0002bbd0: 7365 6c66 2e6f 7264 6572 203d 206f 7264  self.order = ord
-0002bbe0: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
-0002bbf0: 7061 6765 5f6e 756d 6265 7220 3d20 7061  page_number = pa
-0002bc00: 6765 5f6e 756d 6265 720a 2020 2020 2020  ge_number.      
-0002bc10: 2020 7365 6c66 2e70 6167 655f 7369 7a65    self.page_size
-0002bc20: 203d 2070 6167 655f 7369 7a65 0a20 2020   = page_size.   
-0002bc30: 2020 2020 2073 656c 662e 736f 7274 5f62       self.sort_b
-0002bc40: 7920 3d20 736f 7274 5f62 790a 2020 2020  y = sort_by.    
-0002bc50: 2020 2020 7365 6c66 2e73 6f75 7263 655f      self.source_
-0002bc60: 6964 203d 2073 6f75 7263 655f 6964 0a20  id = source_id. 
-0002bc70: 2020 2020 2020 2073 656c 662e 736f 7572         self.sour
-0002bc80: 6365 5f74 7970 6520 3d20 736f 7572 6365  ce_type = source
-0002bc90: 5f74 7970 650a 2020 2020 2020 2020 7365  _type.        se
-0002bca0: 6c66 2e73 7461 7274 5f74 696d 6520 3d20  lf.start_time = 
-0002bcb0: 7374 6172 745f 7469 6d65 0a20 2020 2020  start_time.     
-0002bcc0: 2020 2073 656c 662e 7374 6174 7573 203d     self.status =
-0002bcd0: 2073 7461 7475 730a 2020 2020 2020 2020   status.        
-0002bce0: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
-0002bcf0: 5f69 6420 3d20 7465 6e73 6f72 626f 6172  _id = tensorboar
-0002bd00: 645f 6964 0a20 2020 2020 2020 2073 656c  d_id.        sel
-0002bd10: 662e 7665 7262 6f73 6520 3d20 7665 7262  f.verbose = verb
-0002bd20: 6f73 650a 2020 2020 2020 2020 7365 6c66  ose.        self
-0002bd30: 2e77 6f72 6b73 7061 6365 5f69 6420 3d20  .workspace_id = 
-0002bd40: 776f 726b 7370 6163 655f 6964 0a0a 2020  workspace_id..  
-0002bd50: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0002bd60: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-0002bd70: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-0002bd80: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-0002bd90: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-0002bda0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0002bdb0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0002bdc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002bdd0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0002bde0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0002bdf0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002be00: 6966 2073 656c 662e 6469 7370 6c61 795f  if self.display_
-0002be10: 6e61 6d65 2069 7320 6e6f 7420 4e6f 6e65  name is not None
-0002be20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002be30: 7375 6c74 5b27 4469 7370 6c61 794e 616d  sult['DisplayNam
-0002be40: 6527 5d20 3d20 7365 6c66 2e64 6973 706c  e'] = self.displ
-0002be50: 6179 5f6e 616d 650a 2020 2020 2020 2020  ay_name.        
-0002be60: 6966 2073 656c 662e 656e 645f 7469 6d65  if self.end_time
-0002be70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002be80: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002be90: 5b27 456e 6454 696d 6527 5d20 3d20 7365  ['EndTime'] = se
-0002bea0: 6c66 2e65 6e64 5f74 696d 650a 2020 2020  lf.end_time.    
-0002beb0: 2020 2020 6966 2073 656c 662e 6a6f 625f      if self.job_
-0002bec0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0002bed0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002bee0: 6c74 5b27 4a6f 6249 6427 5d20 3d20 7365  lt['JobId'] = se
-0002bef0: 6c66 2e6a 6f62 5f69 640a 2020 2020 2020  lf.job_id.      
-0002bf00: 2020 6966 2073 656c 662e 6f72 6465 7220    if self.order 
-0002bf10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002bf20: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002bf30: 274f 7264 6572 275d 203d 2073 656c 662e  'Order'] = self.
-0002bf40: 6f72 6465 720a 2020 2020 2020 2020 6966  order.        if
-0002bf50: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
-0002bf60: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-0002bf70: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002bf80: 745b 2750 6167 654e 756d 6265 7227 5d20  t['PageNumber'] 
-0002bf90: 3d20 7365 6c66 2e70 6167 655f 6e75 6d62  = self.page_numb
-0002bfa0: 6572 0a20 2020 2020 2020 2069 6620 7365  er.        if se
-0002bfb0: 6c66 2e70 6167 655f 7369 7a65 2069 7320  lf.page_size is 
-0002bfc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002bfd0: 2020 2020 2020 7265 7375 6c74 5b27 5061        result['Pa
-0002bfe0: 6765 5369 7a65 275d 203d 2073 656c 662e  geSize'] = self.
-0002bff0: 7061 6765 5f73 697a 650a 2020 2020 2020  page_size.      
-0002c000: 2020 6966 2073 656c 662e 736f 7274 5f62    if self.sort_b
-0002c010: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-0002c020: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002c030: 745b 2753 6f72 7442 7927 5d20 3d20 7365  t['SortBy'] = se
-0002c040: 6c66 2e73 6f72 745f 6279 0a20 2020 2020  lf.sort_by.     
-0002c050: 2020 2069 6620 7365 6c66 2e73 6f75 7263     if self.sourc
-0002c060: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
-0002c070: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002c080: 7375 6c74 5b27 536f 7572 6365 4964 275d  sult['SourceId']
-0002c090: 203d 2073 656c 662e 736f 7572 6365 5f69   = self.source_i
-0002c0a0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-0002c0b0: 662e 736f 7572 6365 5f74 7970 6520 6973  f.source_type is
-0002c0c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002c0d0: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
-0002c0e0: 6f75 7263 6554 7970 6527 5d20 3d20 7365  ourceType'] = se
-0002c0f0: 6c66 2e73 6f75 7263 655f 7479 7065 0a20  lf.source_type. 
-0002c100: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0002c110: 7461 7274 5f74 696d 6520 6973 206e 6f74  tart_time is not
-0002c120: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002c130: 2020 2072 6573 756c 745b 2753 7461 7274     result['Start
-0002c140: 5469 6d65 275d 203d 2073 656c 662e 7374  Time'] = self.st
-0002c150: 6172 745f 7469 6d65 0a20 2020 2020 2020  art_time.       
-0002c160: 2069 6620 7365 6c66 2e73 7461 7475 7320   if self.status 
-0002c170: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002c180: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002c190: 2753 7461 7475 7327 5d20 3d20 7365 6c66  'Status'] = self
-0002c1a0: 2e73 7461 7475 730a 2020 2020 2020 2020  .status.        
-0002c1b0: 6966 2073 656c 662e 7465 6e73 6f72 626f  if self.tensorbo
-0002c1c0: 6172 645f 6964 2069 7320 6e6f 7420 4e6f  ard_id is not No
-0002c1d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002c1e0: 7265 7375 6c74 5b27 5465 6e73 6f72 626f  result['Tensorbo
-0002c1f0: 6172 6449 6427 5d20 3d20 7365 6c66 2e74  ardId'] = self.t
-0002c200: 656e 736f 7262 6f61 7264 5f69 640a 2020  ensorboard_id.  
-0002c210: 2020 2020 2020 6966 2073 656c 662e 7665        if self.ve
-0002c220: 7262 6f73 6520 6973 206e 6f74 204e 6f6e  rbose is not Non
-0002c230: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002c240: 6573 756c 745b 2756 6572 626f 7365 275d  esult['Verbose']
-0002c250: 203d 2073 656c 662e 7665 7262 6f73 650a   = self.verbose.
-0002c260: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002c270: 776f 726b 7370 6163 655f 6964 2069 7320  workspace_id is 
-0002c280: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002c290: 2020 2020 2020 7265 7375 6c74 5b27 576f        result['Wo
-0002c2a0: 726b 7370 6163 6549 6427 5d20 3d20 7365  rkspaceId'] = se
-0002c2b0: 6c66 2e77 6f72 6b73 7061 6365 5f69 640a  lf.workspace_id.
-0002c2c0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0002c2d0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-0002c2e0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-0002c2f0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-0002c300: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-0002c310: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0002c320: 6620 6d2e 6765 7428 2744 6973 706c 6179  f m.get('Display
-0002c330: 4e61 6d65 2729 2069 7320 6e6f 7420 4e6f  Name') is not No
-0002c340: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002c350: 7365 6c66 2e64 6973 706c 6179 5f6e 616d  self.display_nam
-0002c360: 6520 3d20 6d2e 6765 7428 2744 6973 706c  e = m.get('Displ
-0002c370: 6179 4e61 6d65 2729 0a20 2020 2020 2020  ayName').       
-0002c380: 2069 6620 6d2e 6765 7428 2745 6e64 5469   if m.get('EndTi
-0002c390: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
-0002c3a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002c3b0: 6c66 2e65 6e64 5f74 696d 6520 3d20 6d2e  lf.end_time = m.
-0002c3c0: 6765 7428 2745 6e64 5469 6d65 2729 0a20  get('EndTime'). 
-0002c3d0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002c3e0: 274a 6f62 4964 2729 2069 7320 6e6f 7420  'JobId') is not 
-0002c3f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002c400: 2020 7365 6c66 2e6a 6f62 5f69 6420 3d20    self.job_id = 
-0002c410: 6d2e 6765 7428 274a 6f62 4964 2729 0a20  m.get('JobId'). 
-0002c420: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002c430: 274f 7264 6572 2729 2069 7320 6e6f 7420  'Order') is not 
-0002c440: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002c450: 2020 7365 6c66 2e6f 7264 6572 203d 206d    self.order = m
-0002c460: 2e67 6574 2827 4f72 6465 7227 290a 2020  .get('Order').  
-0002c470: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002c480: 5061 6765 4e75 6d62 6572 2729 2069 7320  PageNumber') is 
-0002c490: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002c4a0: 2020 2020 2020 7365 6c66 2e70 6167 655f        self.page_
-0002c4b0: 6e75 6d62 6572 203d 206d 2e67 6574 2827  number = m.get('
-0002c4c0: 5061 6765 4e75 6d62 6572 2729 0a20 2020  PageNumber').   
-0002c4d0: 2020 2020 2069 6620 6d2e 6765 7428 2750       if m.get('P
-0002c4e0: 6167 6553 697a 6527 2920 6973 206e 6f74  ageSize') is not
-0002c4f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002c500: 2020 2073 656c 662e 7061 6765 5f73 697a     self.page_siz
-0002c510: 6520 3d20 6d2e 6765 7428 2750 6167 6553  e = m.get('PageS
-0002c520: 697a 6527 290a 2020 2020 2020 2020 6966  ize').        if
-0002c530: 206d 2e67 6574 2827 536f 7274 4279 2729   m.get('SortBy')
-0002c540: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002c550: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0002c560: 6f72 745f 6279 203d 206d 2e67 6574 2827  ort_by = m.get('
-0002c570: 536f 7274 4279 2729 0a20 2020 2020 2020  SortBy').       
-0002c580: 2069 6620 6d2e 6765 7428 2753 6f75 7263   if m.get('Sourc
-0002c590: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
-0002c5a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002c5b0: 656c 662e 736f 7572 6365 5f69 6420 3d20  elf.source_id = 
-0002c5c0: 6d2e 6765 7428 2753 6f75 7263 6549 6427  m.get('SourceId'
-0002c5d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002c5e0: 6574 2827 536f 7572 6365 5479 7065 2729  et('SourceType')
-0002c5f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002c600: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0002c610: 6f75 7263 655f 7479 7065 203d 206d 2e67  ource_type = m.g
-0002c620: 6574 2827 536f 7572 6365 5479 7065 2729  et('SourceType')
-0002c630: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002c640: 7428 2753 7461 7274 5469 6d65 2729 2069  t('StartTime') i
-0002c650: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002c660: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0002c670: 7274 5f74 696d 6520 3d20 6d2e 6765 7428  rt_time = m.get(
-0002c680: 2753 7461 7274 5469 6d65 2729 0a20 2020  'StartTime').   
-0002c690: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
-0002c6a0: 7461 7475 7327 2920 6973 206e 6f74 204e  tatus') is not N
-0002c6b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002c6c0: 2073 656c 662e 7374 6174 7573 203d 206d   self.status = m
-0002c6d0: 2e67 6574 2827 5374 6174 7573 2729 0a20  .get('Status'). 
-0002c6e0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002c6f0: 2754 656e 736f 7262 6f61 7264 4964 2729  'TensorboardId')
-0002c700: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002c710: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-0002c720: 656e 736f 7262 6f61 7264 5f69 6420 3d20  ensorboard_id = 
-0002c730: 6d2e 6765 7428 2754 656e 736f 7262 6f61  m.get('Tensorboa
-0002c740: 7264 4964 2729 0a20 2020 2020 2020 2069  rdId').        i
-0002c750: 6620 6d2e 6765 7428 2756 6572 626f 7365  f m.get('Verbose
-0002c760: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002c770: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002c780: 2e76 6572 626f 7365 203d 206d 2e67 6574  .verbose = m.get
-0002c790: 2827 5665 7262 6f73 6527 290a 2020 2020  ('Verbose').    
-0002c7a0: 2020 2020 6966 206d 2e67 6574 2827 576f      if m.get('Wo
-0002c7b0: 726b 7370 6163 6549 6427 2920 6973 206e  rkspaceId') is n
-0002c7c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002c7d0: 2020 2020 2073 656c 662e 776f 726b 7370       self.worksp
-0002c7e0: 6163 655f 6964 203d 206d 2e67 6574 2827  ace_id = m.get('
-0002c7f0: 576f 726b 7370 6163 6549 6427 290a 2020  WorkspaceId').  
-0002c800: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0002c810: 660a 0a0a 636c 6173 7320 4c69 7374 5465  f...class ListTe
-0002c820: 6e73 6f72 626f 6172 6473 5265 7370 6f6e  nsorboardsRespon
-0002c830: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
-0002c840: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0002c850: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0002c860: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
-0002c870: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
-0002c880: 2c0a 2020 2020 2020 2020 7465 6e73 6f72  ,.        tensor
-0002c890: 626f 6172 6473 3a20 4c69 7374 5b54 656e  boards: List[Ten
-0002c8a0: 736f 7262 6f61 7264 5d20 3d20 4e6f 6e65  sorboard] = None
-0002c8b0: 2c0a 2020 2020 2020 2020 746f 7461 6c5f  ,.        total_
-0002c8c0: 636f 756e 743a 2069 6e74 203d 204e 6f6e  count: int = Non
-0002c8d0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-0002c8e0: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
-0002c8f0: 6420 3d20 7265 7175 6573 745f 6964 0a20  d = request_id. 
-0002c900: 2020 2020 2020 2073 656c 662e 7465 6e73         self.tens
-0002c910: 6f72 626f 6172 6473 203d 2074 656e 736f  orboards = tenso
-0002c920: 7262 6f61 7264 730a 2020 2020 2020 2020  rboards.        
-0002c930: 7365 6c66 2e74 6f74 616c 5f63 6f75 6e74  self.total_count
-0002c940: 203d 2074 6f74 616c 5f63 6f75 6e74 0a0a   = total_count..
-0002c950: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0002c960: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002c970: 6966 2073 656c 662e 7465 6e73 6f72 626f  if self.tensorbo
-0002c980: 6172 6473 3a0a 2020 2020 2020 2020 2020  ards:.          
-0002c990: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
-0002c9a0: 7465 6e73 6f72 626f 6172 6473 3a0a 2020  tensorboards:.  
-0002c9b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0002c9c0: 206b 3a0a 2020 2020 2020 2020 2020 2020   k:.            
-0002c9d0: 2020 2020 2020 2020 6b2e 7661 6c69 6461          k.valida
-0002c9e0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-0002c9f0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0002ca00: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0002ca10: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-0002ca20: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0002ca30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002ca40: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0002ca50: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0002ca60: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0002ca70: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-0002ca80: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-0002ca90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002caa0: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
-0002cab0: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
-0002cac0: 5f69 640a 2020 2020 2020 2020 7265 7375  _id.        resu
-0002cad0: 6c74 5b27 5465 6e73 6f72 626f 6172 6473  lt['Tensorboards
-0002cae0: 275d 203d 205b 5d0a 2020 2020 2020 2020  '] = [].        
-0002caf0: 6966 2073 656c 662e 7465 6e73 6f72 626f  if self.tensorbo
-0002cb00: 6172 6473 2069 7320 6e6f 7420 4e6f 6e65  ards is not None
-0002cb10: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0002cb20: 7220 6b20 696e 2073 656c 662e 7465 6e73  r k in self.tens
-0002cb30: 6f72 626f 6172 6473 3a0a 2020 2020 2020  orboards:.      
-0002cb40: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002cb50: 5b27 5465 6e73 6f72 626f 6172 6473 275d  ['Tensorboards']
-0002cb60: 2e61 7070 656e 6428 6b2e 746f 5f6d 6170  .append(k.to_map
-0002cb70: 2829 2069 6620 6b20 656c 7365 204e 6f6e  () if k else Non
-0002cb80: 6529 0a20 2020 2020 2020 2069 6620 7365  e).        if se
-0002cb90: 6c66 2e74 6f74 616c 5f63 6f75 6e74 2069  lf.total_count i
-0002cba0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002cbb0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002cbc0: 546f 7461 6c43 6f75 6e74 275d 203d 2073  TotalCount'] = s
-0002cbd0: 656c 662e 746f 7461 6c5f 636f 756e 740a  elf.total_count.
-0002cbe0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0002cbf0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-0002cc00: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-0002cc10: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-0002cc20: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-0002cc30: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0002cc40: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
-0002cc50: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-0002cc60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002cc70: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-0002cc80: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-0002cc90: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-0002cca0: 7465 6e73 6f72 626f 6172 6473 203d 205b  tensorboards = [
-0002ccb0: 5d0a 2020 2020 2020 2020 6966 206d 2e67  ].        if m.g
-0002ccc0: 6574 2827 5465 6e73 6f72 626f 6172 6473  et('Tensorboards
-0002ccd0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002cce0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0002ccf0: 6b20 696e 206d 2e67 6574 2827 5465 6e73  k in m.get('Tens
-0002cd00: 6f72 626f 6172 6473 2729 3a0a 2020 2020  orboards'):.    
-0002cd10: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0002cd20: 5f6d 6f64 656c 203d 2054 656e 736f 7262  _model = Tensorb
-0002cd30: 6f61 7264 2829 0a20 2020 2020 2020 2020  oard().         
-0002cd40: 2020 2020 2020 2073 656c 662e 7465 6e73         self.tens
-0002cd50: 6f72 626f 6172 6473 2e61 7070 656e 6428  orboards.append(
-0002cd60: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-0002cd70: 6d61 7028 6b29 290a 2020 2020 2020 2020  map(k)).        
-0002cd80: 6966 206d 2e67 6574 2827 546f 7461 6c43  if m.get('TotalC
-0002cd90: 6f75 6e74 2729 2069 7320 6e6f 7420 4e6f  ount') is not No
-0002cda0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002cdb0: 7365 6c66 2e74 6f74 616c 5f63 6f75 6e74  self.total_count
-0002cdc0: 203d 206d 2e67 6574 2827 546f 7461 6c43   = m.get('TotalC
-0002cdd0: 6f75 6e74 2729 0a20 2020 2020 2020 2072  ount').        r
-0002cde0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-0002cdf0: 7373 204c 6973 7454 656e 736f 7262 6f61  ss ListTensorboa
-0002ce00: 7264 7352 6573 706f 6e73 6528 5465 614d  rdsResponse(TeaM
-0002ce10: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002ce20: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0002ce30: 2073 656c 662c 0a20 2020 2020 2020 2068   self,.        h
-0002ce40: 6561 6465 7273 3a20 4469 6374 5b73 7472  eaders: Dict[str
-0002ce50: 2c20 7374 725d 203d 204e 6f6e 652c 0a20  , str] = None,. 
-0002ce60: 2020 2020 2020 2073 7461 7475 735f 636f         status_co
-0002ce70: 6465 3a20 696e 7420 3d20 4e6f 6e65 2c0a  de: int = None,.
-0002ce80: 2020 2020 2020 2020 626f 6479 3a20 4c69          body: Li
-0002ce90: 7374 5465 6e73 6f72 626f 6172 6473 5265  stTensorboardsRe
-0002cea0: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
-0002ceb0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-0002cec0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-0002ced0: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
-0002cee0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0002cef0: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
-0002cf00: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0002cf10: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
-0002cf20: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0002cf30: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
-0002cf40: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
-0002cf50: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
-0002cf60: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-0002cf70: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
-0002cf80: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
-0002cf90: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
-0002cfa0: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
-0002cfb0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
-0002cfc0: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
-0002cfd0: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
-0002cfe0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-0002cff0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002d000: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
-0002d010: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-0002d020: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-0002d030: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-0002d040: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0002d050: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0002d060: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002d070: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0002d080: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0002d090: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002d0a0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-0002d0b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002d0c0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002d0d0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-0002d0e0: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-0002d0f0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-0002d100: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-0002d110: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002d120: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-0002d130: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-0002d140: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-0002d150: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-0002d160: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002d170: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-0002d180: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-0002d190: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0002d1a0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0002d1b0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0002d1c0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-0002d1d0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-0002d1e0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-0002d1f0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002d200: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
-0002d210: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002d220: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-0002d230: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
-0002d240: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
-0002d250: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-0002d260: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-0002d270: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002d280: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-0002d290: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-0002d2a0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-0002d2b0: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
-0002d2c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002d2d0: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-0002d2e0: 203d 204c 6973 7454 656e 736f 7262 6f61   = ListTensorboa
-0002d2f0: 7264 7352 6573 706f 6e73 6542 6f64 7928  rdsResponseBody(
-0002d300: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0002d310: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-0002d320: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-0002d330: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-0002d340: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0002d350: 6c61 7373 2053 7461 7274 5465 6e73 6f72  lass StartTensor
-0002d360: 626f 6172 6452 6571 7565 7374 2854 6561  boardRequest(Tea
-0002d370: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0002d380: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-0002d390: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0002d3a0: 776f 726b 7370 6163 655f 6964 3a20 7374  workspace_id: st
-0002d3b0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 293a  r = None,.    ):
-0002d3c0: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
-0002d3d0: 726b 7370 6163 655f 6964 203d 2077 6f72  rkspace_id = wor
-0002d3e0: 6b73 7061 6365 5f69 640a 0a20 2020 2064  kspace_id..    d
-0002d3f0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0002d400: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0002d410: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0002d420: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0002d430: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-0002d440: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0002d450: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0002d460: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002d470: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0002d480: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0002d490: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0002d4a0: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
-0002d4b0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-0002d4c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002d4d0: 745b 2757 6f72 6b73 7061 6365 4964 275d  t['WorkspaceId']
-0002d4e0: 203d 2073 656c 662e 776f 726b 7370 6163   = self.workspac
-0002d4f0: 655f 6964 0a20 2020 2020 2020 2072 6574  e_id.        ret
-0002d500: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0002d510: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0002d520: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-0002d530: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0002d540: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0002d550: 2020 2020 6966 206d 2e67 6574 2827 576f      if m.get('Wo
-0002d560: 726b 7370 6163 6549 6427 2920 6973 206e  rkspaceId') is n
-0002d570: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002d580: 2020 2020 2073 656c 662e 776f 726b 7370       self.worksp
-0002d590: 6163 655f 6964 203d 206d 2e67 6574 2827  ace_id = m.get('
-0002d5a0: 576f 726b 7370 6163 6549 6427 290a 2020  WorkspaceId').  
-0002d5b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0002d5c0: 660a 0a0a 636c 6173 7320 5374 6172 7454  f...class StartT
-0002d5d0: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
-0002d5e0: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
-0002d5f0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0002d600: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0002d610: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
-0002d620: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
-0002d630: 2c0a 2020 2020 2020 2020 7465 6e73 6f72  ,.        tensor
-0002d640: 626f 6172 645f 6964 3a20 7374 7220 3d20  board_id: str = 
-0002d650: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0002d660: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-0002d670: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
-0002d680: 640a 2020 2020 2020 2020 7365 6c66 2e74  d.        self.t
-0002d690: 656e 736f 7262 6f61 7264 5f69 6420 3d20  ensorboard_id = 
-0002d6a0: 7465 6e73 6f72 626f 6172 645f 6964 0a0a  tensorboard_id..
-0002d6b0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0002d6c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002d6d0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-0002d6e0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0002d6f0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0002d700: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-0002d710: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0002d720: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002d730: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0002d740: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0002d750: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0002d760: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-0002d770: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-0002d780: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002d790: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
-0002d7a0: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
-0002d7b0: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-0002d7c0: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
-0002d7d0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0002d7e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002d7f0: 6c74 5b27 5465 6e73 6f72 626f 6172 6449  lt['TensorboardI
-0002d800: 6427 5d20 3d20 7365 6c66 2e74 656e 736f  d'] = self.tenso
-0002d810: 7262 6f61 7264 5f69 640a 2020 2020 2020  rboard_id.      
-0002d820: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0002d830: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0002d840: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-0002d850: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-0002d860: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-0002d870: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002d880: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
-0002d890: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002d8a0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
-0002d8b0: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
-0002d8c0: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
-0002d8d0: 2020 2020 2069 6620 6d2e 6765 7428 2754       if m.get('T
-0002d8e0: 656e 736f 7262 6f61 7264 4964 2729 2069  ensorboardId') i
-0002d8f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002d900: 2020 2020 2020 2020 7365 6c66 2e74 656e          self.ten
-0002d910: 736f 7262 6f61 7264 5f69 6420 3d20 6d2e  sorboard_id = m.
-0002d920: 6765 7428 2754 656e 736f 7262 6f61 7264  get('Tensorboard
-0002d930: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
-0002d940: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-0002d950: 2053 7461 7274 5465 6e73 6f72 626f 6172   StartTensorboar
-0002d960: 6452 6573 706f 6e73 6528 5465 614d 6f64  dResponse(TeaMod
-0002d970: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-0002d980: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0002d990: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
-0002d9a0: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
-0002d9b0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0002d9c0: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
-0002d9d0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
-0002d9e0: 2020 2020 2020 626f 6479 3a20 5374 6172        body: Star
-0002d9f0: 7454 656e 736f 7262 6f61 7264 5265 7370  tTensorboardResp
-0002da00: 6f6e 7365 426f 6479 203d 204e 6f6e 652c  onseBody = None,
-0002da10: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-0002da20: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
-0002da30: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
-0002da40: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0002da50: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
-0002da60: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-0002da70: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
-0002da80: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0002da90: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
-0002daa0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
-0002dab0: 656c 662e 6865 6164 6572 732c 2027 6865  elf.headers, 'he
-0002dac0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-0002dad0: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-0002dae0: 7175 6972 6564 2873 656c 662e 7374 6174  quired(self.stat
-0002daf0: 7573 5f63 6f64 652c 2027 7374 6174 7573  us_code, 'status
-0002db00: 5f63 6f64 6527 290a 2020 2020 2020 2020  _code').        
-0002db10: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
-0002db20: 7175 6972 6564 2873 656c 662e 626f 6479  quired(self.body
-0002db30: 2c20 2762 6f64 7927 290a 2020 2020 2020  , 'body').      
-0002db40: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
-0002db50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002db60: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
-0002db70: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-0002db80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002db90: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-0002dba0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0002dbb0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-0002dbc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002dbd0: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-0002dbe0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-0002dbf0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0002dc00: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
-0002dc10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002dc20: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
-0002dc30: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
-0002dc40: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
-0002dc50: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
-0002dc60: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
-0002dc70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002dc80: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
-0002dc90: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
-0002dca0: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
-0002dcb0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
-0002dcc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002dcd0: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
-0002dce0: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
-0002dcf0: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
-0002dd00: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-0002dd10: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-0002dd20: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
-0002dd30: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0002dd40: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0002dd50: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002dd60: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
-0002dd70: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002dd80: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-0002dd90: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-0002dda0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0002ddb0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-0002ddc0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002ddd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002dde0: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-0002ddf0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-0002de00: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002de10: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-0002de20: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002de30: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-0002de40: 2053 7461 7274 5465 6e73 6f72 626f 6172   StartTensorboar
-0002de50: 6452 6573 706f 6e73 6542 6f64 7928 290a  dResponseBody().
-0002de60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002de70: 2e62 6f64 7920 3d20 7465 6d70 5f6d 6f64  .body = temp_mod
-0002de80: 656c 2e66 726f 6d5f 6d61 7028 6d5b 2762  el.from_map(m['b
-0002de90: 6f64 7927 5d29 0a20 2020 2020 2020 2072  ody']).        r
-0002dea0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-0002deb0: 7373 2053 746f 704a 6f62 5265 7370 6f6e  ss StopJobRespon
-0002dec0: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
-0002ded0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0002dee0: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0002def0: 2c0a 2020 2020 2020 2020 6a6f 625f 6964  ,.        job_id
-0002df00: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0002df10: 2020 2020 2020 7265 7175 6573 745f 6964        request_id
-0002df20: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0002df30: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-0002df40: 662e 6a6f 625f 6964 203d 206a 6f62 5f69  f.job_id = job_i
-0002df50: 640a 2020 2020 2020 2020 7365 6c66 2e72  d.        self.r
-0002df60: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
-0002df70: 6573 745f 6964 0a0a 2020 2020 6465 6620  est_id..    def 
-0002df80: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
-0002df90: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0002dfa0: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0002dfb0: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0002dfc0: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-0002dfd0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0002dfe0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0002dff0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0002e000: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0002e010: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0002e020: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0002e030: 662e 6a6f 625f 6964 2069 7320 6e6f 7420  f.job_id is not 
-0002e040: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002e050: 2020 7265 7375 6c74 5b27 4a6f 6249 6427    result['JobId'
-0002e060: 5d20 3d20 7365 6c66 2e6a 6f62 5f69 640a  ] = self.job_id.
-0002e070: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002e080: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
-0002e090: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002e0a0: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
-0002e0b0: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
-0002e0c0: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
-0002e0d0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0002e0e0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0002e0f0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-0002e100: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-0002e110: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-0002e120: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002e130: 7428 274a 6f62 4964 2729 2069 7320 6e6f  t('JobId') is no
-0002e140: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002e150: 2020 2020 7365 6c66 2e6a 6f62 5f69 6420      self.job_id 
-0002e160: 3d20 6d2e 6765 7428 274a 6f62 4964 2729  = m.get('JobId')
-0002e170: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002e180: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
-0002e190: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002e1a0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
-0002e1b0: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
-0002e1c0: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
-0002e1d0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0002e1e0: 0a0a 0a63 6c61 7373 2053 746f 704a 6f62  ...class StopJob
-0002e1f0: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
-0002e200: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-0002e210: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0002e220: 6c66 2c0a 2020 2020 2020 2020 6865 6164  lf,.        head
-0002e230: 6572 733a 2044 6963 745b 7374 722c 2073  ers: Dict[str, s
-0002e240: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
-0002e250: 2020 2020 7374 6174 7573 5f63 6f64 653a      status_code:
-0002e260: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-0002e270: 2020 2020 2062 6f64 793a 2053 746f 704a       body: StopJ
-0002e280: 6f62 5265 7370 6f6e 7365 426f 6479 203d  obResponseBody =
-0002e290: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
-0002e2a0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-0002e2b0: 7273 203d 2068 6561 6465 7273 0a20 2020  rs = headers.   
-0002e2c0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-0002e2d0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-0002e2e0: 6f64 650a 2020 2020 2020 2020 7365 6c66  ode.        self
-0002e2f0: 2e62 6f64 7920 3d20 626f 6479 0a0a 2020  .body = body..  
-0002e300: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0002e310: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-0002e320: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-0002e330: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
-0002e340: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
-0002e350: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0002e360: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-0002e370: 662e 7374 6174 7573 5f63 6f64 652c 2027  f.status_code, '
-0002e380: 7374 6174 7573 5f63 6f64 6527 290a 2020  status_code').  
-0002e390: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0002e3a0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-0002e3b0: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
-0002e3c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002e3d0: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
-0002e3e0: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
-0002e3f0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
-0002e400: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0002e410: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0002e420: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-0002e430: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0002e440: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002e450: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0002e460: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0002e470: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0002e480: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
-0002e490: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-0002e4a0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002e4b0: 756c 745b 2768 6561 6465 7273 275d 203d  ult['headers'] =
-0002e4c0: 2073 656c 662e 6865 6164 6572 730a 2020   self.headers.  
-0002e4d0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-0002e4e0: 6174 7573 5f63 6f64 6520 6973 206e 6f74  atus_code is not
-0002e4f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002e500: 2020 2072 6573 756c 745b 2773 7461 7475     result['statu
-0002e510: 7343 6f64 6527 5d20 3d20 7365 6c66 2e73  sCode'] = self.s
-0002e520: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-0002e530: 2020 2069 6620 7365 6c66 2e62 6f64 7920     if self.body 
-0002e540: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002e550: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002e560: 2762 6f64 7927 5d20 3d20 7365 6c66 2e62  'body'] = self.b
-0002e570: 6f64 792e 746f 5f6d 6170 2829 0a20 2020  ody.to_map().   
-0002e580: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0002e590: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-0002e5a0: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-0002e5b0: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-0002e5c0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0002e5d0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0002e5e0: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
-0002e5f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002e600: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-0002e610: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
-0002e620: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
-0002e630: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
-0002e640: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
-0002e650: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002e660: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0002e670: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
-0002e680: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
-0002e690: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
-0002e6a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002e6b0: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-0002e6c0: 6f64 656c 203d 2053 746f 704a 6f62 5265  odel = StopJobRe
-0002e6d0: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
-0002e6e0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0002e6f0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-0002e700: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-0002e710: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-0002e720: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-0002e730: 5374 6f70 5465 6e73 6f72 626f 6172 6452  StopTensorboardR
-0002e740: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
-0002e750: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0002e760: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0002e770: 2c0a 2020 2020 2020 2020 776f 726b 7370  ,.        worksp
-0002e780: 6163 655f 6964 3a20 7374 7220 3d20 4e6f  ace_id: str = No
-0002e790: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0002e7a0: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
-0002e7b0: 655f 6964 203d 2077 6f72 6b73 7061 6365  e_id = workspace
-0002e7c0: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
-0002e7d0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0002e7e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-0002e7f0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-0002e800: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-0002e810: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-0002e820: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0002e830: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002e840: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002e850: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0002e860: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0002e870: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
-0002e880: 6f72 6b73 7061 6365 5f69 6420 6973 206e  orkspace_id is n
-0002e890: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002e8a0: 2020 2020 2072 6573 756c 745b 2757 6f72       result['Wor
-0002e8b0: 6b73 7061 6365 4964 275d 203d 2073 656c  kspaceId'] = sel
-0002e8c0: 662e 776f 726b 7370 6163 655f 6964 0a20  f.workspace_id. 
-0002e8d0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002e8e0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0002e8f0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-0002e900: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-0002e910: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0002e920: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0002e930: 206d 2e67 6574 2827 576f 726b 7370 6163   m.get('Workspac
-0002e940: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
-0002e950: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002e960: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-0002e970: 203d 206d 2e67 6574 2827 576f 726b 7370   = m.get('Worksp
-0002e980: 6163 6549 6427 290a 2020 2020 2020 2020  aceId').        
-0002e990: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-0002e9a0: 6173 7320 5374 6f70 5465 6e73 6f72 626f  ass StopTensorbo
-0002e9b0: 6172 6452 6573 706f 6e73 6542 6f64 7928  ardResponseBody(
-0002e9c0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0002e9d0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0002e9e0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002e9f0: 2020 2072 6571 7565 7374 5f69 643a 2073     request_id: s
-0002ea00: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0002ea10: 2020 2074 656e 736f 7262 6f61 7264 5f69     tensorboard_i
-0002ea20: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-0002ea30: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-0002ea40: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-0002ea50: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
-0002ea60: 2020 2073 656c 662e 7465 6e73 6f72 626f     self.tensorbo
-0002ea70: 6172 645f 6964 203d 2074 656e 736f 7262  ard_id = tensorb
-0002ea80: 6f61 7264 5f69 640a 0a20 2020 2064 6566  oard_id..    def
-0002ea90: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0002eaa0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0002eab0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0002eac0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0002ead0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-0002eae0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0002eaf0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0002eb00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002eb10: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0002eb20: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0002eb30: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0002eb40: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
-0002eb50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002eb60: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-0002eb70: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
-0002eb80: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
-0002eb90: 2020 2020 2069 6620 7365 6c66 2e74 656e       if self.ten
-0002eba0: 736f 7262 6f61 7264 5f69 6420 6973 206e  sorboard_id is n
-0002ebb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002ebc0: 2020 2020 2072 6573 756c 745b 2754 656e       result['Ten
-0002ebd0: 736f 7262 6f61 7264 4964 275d 203d 2073  sorboardId'] = s
-0002ebe0: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
-0002ebf0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-0002ec00: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0002ec10: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0002ec20: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-0002ec30: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-0002ec40: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-0002ec50: 2020 6966 206d 2e67 6574 2827 5265 7175    if m.get('Requ
-0002ec60: 6573 7449 6427 2920 6973 206e 6f74 204e  estId') is not N
-0002ec70: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002ec80: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-0002ec90: 203d 206d 2e67 6574 2827 5265 7175 6573   = m.get('Reques
-0002eca0: 7449 6427 290a 2020 2020 2020 2020 6966  tId').        if
-0002ecb0: 206d 2e67 6574 2827 5465 6e73 6f72 626f   m.get('Tensorbo
-0002ecc0: 6172 6449 6427 2920 6973 206e 6f74 204e  ardId') is not N
-0002ecd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002ece0: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
-0002ecf0: 645f 6964 203d 206d 2e67 6574 2827 5465  d_id = m.get('Te
-0002ed00: 6e73 6f72 626f 6172 6449 6427 290a 2020  nsorboardId').  
-0002ed10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0002ed20: 660a 0a0a 636c 6173 7320 5374 6f70 5465  f...class StopTe
-0002ed30: 6e73 6f72 626f 6172 6452 6573 706f 6e73  nsorboardRespons
-0002ed40: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
-0002ed50: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0002ed60: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0002ed70: 2020 2020 2068 6561 6465 7273 3a20 4469       headers: Di
-0002ed80: 6374 5b73 7472 2c20 7374 725d 203d 204e  ct[str, str] = N
-0002ed90: 6f6e 652c 0a20 2020 2020 2020 2073 7461  one,.        sta
-0002eda0: 7475 735f 636f 6465 3a20 696e 7420 3d20  tus_code: int = 
-0002edb0: 4e6f 6e65 2c0a 2020 2020 2020 2020 626f  None,.        bo
-0002edc0: 6479 3a20 5374 6f70 5465 6e73 6f72 626f  dy: StopTensorbo
-0002edd0: 6172 6452 6573 706f 6e73 6542 6f64 7920  ardResponseBody 
-0002ede0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0002edf0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0002ee00: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
-0002ee10: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0002ee20: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-0002ee30: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
-0002ee40: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
-0002ee50: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0002ee60: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-0002ee70: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0002ee80: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
-0002ee90: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
-0002eea0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0002eeb0: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0002eec0: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
-0002eed0: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
-0002eee0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0002eef0: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0002ef00: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
-0002ef10: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002ef20: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
-0002ef30: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
-0002ef40: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-0002ef50: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0002ef60: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0002ef70: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-0002ef80: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-0002ef90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002efa0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-0002efb0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-0002efc0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-0002efd0: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
-0002efe0: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
-0002eff0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002f000: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
-0002f010: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
-0002f020: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0002f030: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
-0002f040: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002f050: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
-0002f060: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
-0002f070: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-0002f080: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-0002f090: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002f0a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002f0b0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
-0002f0c0: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
-0002f0d0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0002f0e0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0002f0f0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-0002f100: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-0002f110: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-0002f120: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0002f130: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-0002f140: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002f150: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-0002f160: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
-0002f170: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-0002f180: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
-0002f190: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
-0002f1a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002f1b0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-0002f1c0: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
-0002f1d0: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
-0002f1e0: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-0002f1f0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002f200: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-0002f210: 6d6f 6465 6c20 3d20 5374 6f70 5465 6e73  model = StopTens
-0002f220: 6f72 626f 6172 6452 6573 706f 6e73 6542  orboardResponseB
-0002f230: 6f64 7928 290a 2020 2020 2020 2020 2020  ody().          
-0002f240: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
-0002f250: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-0002f260: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
-0002f270: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0002f280: 0a0a 0a63 6c61 7373 2055 7064 6174 654a  ...class UpdateJ
-0002f290: 6f62 5265 7175 6573 7428 5465 614d 6f64  obRequest(TeaMod
-0002f2a0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-0002f2b0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-0002f2c0: 656c 662c 0a20 2020 2020 2020 2070 7269  elf,.        pri
-0002f2d0: 6f72 6974 793a 2069 6e74 203d 204e 6f6e  ority: int = Non
-0002f2e0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-0002f2f0: 2020 7365 6c66 2e70 7269 6f72 6974 7920    self.priority 
-0002f300: 3d20 7072 696f 7269 7479 0a0a 2020 2020  = priority..    
-0002f310: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0002f320: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-0002f330: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-0002f340: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002f350: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
-0002f360: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0002f370: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-0002f380: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002f390: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-0002f3a0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-0002f3b0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0002f3c0: 2073 656c 662e 7072 696f 7269 7479 2069   self.priority i
-0002f3d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002f3e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002f3f0: 5072 696f 7269 7479 275d 203d 2073 656c  Priority'] = sel
-0002f400: 662e 7072 696f 7269 7479 0a20 2020 2020  f.priority.     
-0002f410: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-0002f420: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-0002f430: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-0002f440: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-0002f450: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-0002f460: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002f470: 6574 2827 5072 696f 7269 7479 2729 2069  et('Priority') i
-0002f480: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002f490: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
-0002f4a0: 6f72 6974 7920 3d20 6d2e 6765 7428 2750  ority = m.get('P
-0002f4b0: 7269 6f72 6974 7927 290a 2020 2020 2020  riority').      
-0002f4c0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0002f4d0: 636c 6173 7320 5570 6461 7465 4a6f 6252  class UpdateJobR
-0002f4e0: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-0002f4f0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002f500: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0002f510: 2073 656c 662c 0a20 2020 2020 2020 206a   self,.        j
-0002f520: 6f62 5f69 643a 2073 7472 203d 204e 6f6e  ob_id: str = Non
-0002f530: 652c 0a20 2020 2020 2020 2072 6571 7565  e,.        reque
-0002f540: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
-0002f550: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-0002f560: 2020 7365 6c66 2e6a 6f62 5f69 6420 3d20    self.job_id = 
-0002f570: 6a6f 625f 6964 0a20 2020 2020 2020 2073  job_id.        s
-0002f580: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-0002f590: 2072 6571 7565 7374 5f69 640a 0a20 2020   request_id..   
-0002f5a0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0002f5b0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-0002f5c0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-0002f5d0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0002f5e0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-0002f5f0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0002f600: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-0002f610: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002f620: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-0002f630: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0002f640: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0002f650: 6620 7365 6c66 2e6a 6f62 5f69 6420 6973  f self.job_id is
-0002f660: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002f670: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
-0002f680: 6f62 4964 275d 203d 2073 656c 662e 6a6f  obId'] = self.jo
-0002f690: 625f 6964 0a20 2020 2020 2020 2069 6620  b_id.        if 
-0002f6a0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-0002f6b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002f6c0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002f6d0: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
-0002f6e0: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
-0002f6f0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002f700: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0002f710: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-0002f720: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-0002f730: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0002f740: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0002f750: 206d 2e67 6574 2827 4a6f 6249 6427 2920   m.get('JobId') 
-0002f760: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002f770: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
-0002f780: 625f 6964 203d 206d 2e67 6574 2827 4a6f  b_id = m.get('Jo
-0002f790: 6249 6427 290a 2020 2020 2020 2020 6966  bId').        if
-0002f7a0: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
-0002f7b0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-0002f7c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002f7d0: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
-0002f7e0: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-0002f7f0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0002f800: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-0002f810: 6461 7465 4a6f 6252 6573 706f 6e73 6528  dateJobResponse(
-0002f820: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0002f830: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0002f840: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002f850: 2020 2068 6561 6465 7273 3a20 4469 6374     headers: Dict
-0002f860: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
-0002f870: 652c 0a20 2020 2020 2020 2073 7461 7475  e,.        statu
-0002f880: 735f 636f 6465 3a20 696e 7420 3d20 4e6f  s_code: int = No
-0002f890: 6e65 2c0a 2020 2020 2020 2020 626f 6479  ne,.        body
-0002f8a0: 3a20 5570 6461 7465 4a6f 6252 6573 706f  : UpdateJobRespo
-0002f8b0: 6e73 6542 6f64 7920 3d20 4e6f 6e65 2c0a  nseBody = None,.
-0002f8c0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
-0002f8d0: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
-0002f8e0: 6164 6572 730a 2020 2020 2020 2020 7365  aders.        se
-0002f8f0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
-0002f900: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
-0002f910: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-0002f920: 2062 6f64 790a 0a20 2020 2064 6566 2076   body..    def v
-0002f930: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0002f940: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0002f950: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0002f960: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
-0002f970: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
-0002f980: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0002f990: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
-0002f9a0: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
-0002f9b0: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
-0002f9c0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0002f9d0: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
-0002f9e0: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
-0002f9f0: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-0002fa00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002fa10: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-0002fa20: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0002fa30: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0002fa40: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-0002fa50: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0002fa60: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0002fa70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002fa80: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0002fa90: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0002faa0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0002fab0: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-0002fac0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002fad0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-0002fae0: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-0002faf0: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-0002fb00: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
-0002fb10: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
-0002fb20: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002fb30: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
-0002fb40: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
-0002fb50: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
-0002fb60: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-0002fb70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002fb80: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-0002fb90: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-0002fba0: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-0002fbb0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-0002fbc0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-0002fbd0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
-0002fbe0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0002fbf0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0002fc00: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
-0002fc10: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
-0002fc20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002fc30: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-0002fc40: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
-0002fc50: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002fc60: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-0002fc70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002fc80: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0002fc90: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
-0002fca0: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
-0002fcb0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002fcc0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
-0002fcd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002fce0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-0002fcf0: 5570 6461 7465 4a6f 6252 6573 706f 6e73  UpdateJobRespons
-0002fd00: 6542 6f64 7928 290a 2020 2020 2020 2020  eBody().        
-0002fd10: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-0002fd20: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
-0002fd30: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
-0002fd40: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0002fd50: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
-0002fd60: 6554 656e 736f 7262 6f61 7264 5265 7175  eTensorboardRequ
-0002fd70: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
-0002fd80: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0002fd90: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0002fda0: 2020 2020 2020 206d 6178 5f72 756e 6e69         max_runni
-0002fdb0: 6e67 5f74 696d 655f 6d69 6e75 7465 733a  ng_time_minutes:
-0002fdc0: 2069 6e74 203d 204e 6f6e 652c 0a20 2020   int = None,.   
-0002fdd0: 2020 2020 2077 6f72 6b73 7061 6365 5f69       workspace_i
-0002fde0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-0002fdf0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-0002fe00: 6c66 2e6d 6178 5f72 756e 6e69 6e67 5f74  lf.max_running_t
-0002fe10: 696d 655f 6d69 6e75 7465 7320 3d20 6d61  ime_minutes = ma
-0002fe20: 785f 7275 6e6e 696e 675f 7469 6d65 5f6d  x_running_time_m
-0002fe30: 696e 7574 6573 0a20 2020 2020 2020 2073  inutes.        s
-0002fe40: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-0002fe50: 203d 2077 6f72 6b73 7061 6365 5f69 640a   = workspace_id.
-0002fe60: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0002fe70: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0002fe80: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-0002fe90: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-0002fea0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-0002feb0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-0002fec0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-0002fed0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002fee0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-0002fef0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-0002ff00: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0002ff10: 2020 2069 6620 7365 6c66 2e6d 6178 5f72     if self.max_r
-0002ff20: 756e 6e69 6e67 5f74 696d 655f 6d69 6e75  unning_time_minu
-0002ff30: 7465 7320 6973 206e 6f74 204e 6f6e 653a  tes is not None:
-0002ff40: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002ff50: 756c 745b 274d 6178 5275 6e6e 696e 6754  ult['MaxRunningT
-0002ff60: 696d 654d 696e 7574 6573 275d 203d 2073  imeMinutes'] = s
-0002ff70: 656c 662e 6d61 785f 7275 6e6e 696e 675f  elf.max_running_
-0002ff80: 7469 6d65 5f6d 696e 7574 6573 0a20 2020  time_minutes.   
-0002ff90: 2020 2020 2069 6620 7365 6c66 2e77 6f72       if self.wor
-0002ffa0: 6b73 7061 6365 5f69 6420 6973 206e 6f74  kspace_id is not
-0002ffb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002ffc0: 2020 2072 6573 756c 745b 2757 6f72 6b73     result['Works
-0002ffd0: 7061 6365 4964 275d 203d 2073 656c 662e  paceId'] = self.
-0002ffe0: 776f 726b 7370 6163 655f 6964 0a20 2020  workspace_id.   
-0002fff0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00030000: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
-00030010: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
-00030020: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
-00030030: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-00030040: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-00030050: 2e67 6574 2827 4d61 7852 756e 6e69 6e67  .get('MaxRunning
-00030060: 5469 6d65 4d69 6e75 7465 7327 2920 6973  TimeMinutes') is
-00030070: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00030080: 2020 2020 2020 2073 656c 662e 6d61 785f         self.max_
-00030090: 7275 6e6e 696e 675f 7469 6d65 5f6d 696e  running_time_min
-000300a0: 7574 6573 203d 206d 2e67 6574 2827 4d61  utes = m.get('Ma
-000300b0: 7852 756e 6e69 6e67 5469 6d65 4d69 6e75  xRunningTimeMinu
-000300c0: 7465 7327 290a 2020 2020 2020 2020 6966  tes').        if
-000300d0: 206d 2e67 6574 2827 576f 726b 7370 6163   m.get('Workspac
-000300e0: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
-000300f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00030100: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-00030110: 203d 206d 2e67 6574 2827 576f 726b 7370   = m.get('Worksp
-00030120: 6163 6549 6427 290a 2020 2020 2020 2020  aceId').        
-00030130: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-00030140: 6173 7320 5570 6461 7465 5465 6e73 6f72  ass UpdateTensor
-00030150: 626f 6172 6452 6573 706f 6e73 6542 6f64  boardResponseBod
-00030160: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
-00030170: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00030180: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00030190: 2020 2020 2072 6571 7565 7374 5f69 643a       request_id:
-000301a0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-000301b0: 2020 2020 2074 656e 736f 7262 6f61 7264       tensorboard
-000301c0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-000301d0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-000301e0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-000301f0: 3d20 7265 7175 6573 745f 6964 0a20 2020  = request_id.   
-00030200: 2020 2020 2073 656c 662e 7465 6e73 6f72       self.tensor
-00030210: 626f 6172 645f 6964 203d 2074 656e 736f  board_id = tenso
-00030220: 7262 6f61 7264 5f69 640a 0a20 2020 2064  rboard_id..    d
-00030230: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-00030240: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-00030250: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-00030260: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-00030270: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-00030280: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-00030290: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-000302a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000302b0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-000302c0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-000302d0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-000302e0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-000302f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00030300: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00030310: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
-00030320: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
-00030330: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-00030340: 656e 736f 7262 6f61 7264 5f69 6420 6973  ensorboard_id is
-00030350: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00030360: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
-00030370: 656e 736f 7262 6f61 7264 4964 275d 203d  ensorboardId'] =
-00030380: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
-00030390: 645f 6964 0a20 2020 2020 2020 2072 6574  d_id.        ret
-000303a0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000303b0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000303c0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-000303d0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-000303e0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000303f0: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-00030400: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
-00030410: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00030420: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-00030430: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
-00030440: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
-00030450: 6966 206d 2e67 6574 2827 5465 6e73 6f72  if m.get('Tensor
-00030460: 626f 6172 6449 6427 2920 6973 206e 6f74  boardId') is not
-00030470: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00030480: 2020 2073 656c 662e 7465 6e73 6f72 626f     self.tensorbo
-00030490: 6172 645f 6964 203d 206d 2e67 6574 2827  ard_id = m.get('
-000304a0: 5465 6e73 6f72 626f 6172 6449 6427 290a  TensorboardId').
-000304b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000304c0: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
-000304d0: 7465 5465 6e73 6f72 626f 6172 6452 6573  teTensorboardRes
-000304e0: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-000304f0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00030500: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00030510: 0a20 2020 2020 2020 2068 6561 6465 7273  .        headers
-00030520: 3a20 4469 6374 5b73 7472 2c20 7374 725d  : Dict[str, str]
-00030530: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00030540: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
-00030550: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-00030560: 2020 626f 6479 3a20 5570 6461 7465 5465    body: UpdateTe
-00030570: 6e73 6f72 626f 6172 6452 6573 706f 6e73  nsorboardRespons
-00030580: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
-00030590: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-000305a0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-000305b0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-000305c0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-000305d0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-000305e0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-000305f0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
-00030600: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00030610: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00030620: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-00030630: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
-00030640: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
-00030650: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00030660: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
-00030670: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
-00030680: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
-00030690: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-000306a0: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
-000306b0: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
-000306c0: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
-000306d0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-000306e0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
-000306f0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00030700: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00030710: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-00030720: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00030730: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00030740: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00030750: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00030760: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00030770: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00030780: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-00030790: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000307a0: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-000307b0: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-000307c0: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-000307d0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-000307e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000307f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00030800: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-00030810: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00030820: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00030830: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-00030840: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00030850: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-00030860: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-00030870: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-00030880: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00030890: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-000308a0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-000308b0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-000308c0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-000308d0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-000308e0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-000308f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00030900: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-00030910: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-00030920: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00030930: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-00030940: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00030950: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00030960: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-00030970: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-00030980: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00030990: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-000309a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000309b0: 2074 656d 705f 6d6f 6465 6c20 3d20 5570   temp_model = Up
-000309c0: 6461 7465 5465 6e73 6f72 626f 6172 6452  dateTensorboardR
-000309d0: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
-000309e0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-000309f0: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
-00030a00: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
-00030a10: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
-00030a20: 7572 6e20 7365 6c66 0a0a 0a              urn self...
+00026ca0: 0a0a 636c 6173 7320 4765 7454 6f6b 656e  ..class GetToken
+00026cb0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+00026cc0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00026cd0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+00026ce0: 662c 0a20 2020 2020 2020 2065 7870 6972  f,.        expir
+00026cf0: 655f 7469 6d65 3a20 696e 7420 3d20 4e6f  e_time: int = No
+00026d00: 6e65 2c0a 2020 2020 2020 2020 7461 7267  ne,.        targ
+00026d10: 6574 5f69 643a 2073 7472 203d 204e 6f6e  et_id: str = Non
+00026d20: 652c 0a20 2020 2020 2020 2074 6172 6765  e,.        targe
+00026d30: 745f 7479 7065 3a20 7374 7220 3d20 4e6f  t_type: str = No
+00026d40: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+00026d50: 2020 2073 656c 662e 6578 7069 7265 5f74     self.expire_t
+00026d60: 696d 6520 3d20 6578 7069 7265 5f74 696d  ime = expire_tim
+00026d70: 650a 2020 2020 2020 2020 7365 6c66 2e74  e.        self.t
+00026d80: 6172 6765 745f 6964 203d 2074 6172 6765  arget_id = targe
+00026d90: 745f 6964 0a20 2020 2020 2020 2073 656c  t_id.        sel
+00026da0: 662e 7461 7267 6574 5f74 7970 6520 3d20  f.target_type = 
+00026db0: 7461 7267 6574 5f74 7970 650a 0a20 2020  target_type..   
+00026dc0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+00026dd0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+00026de0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+00026df0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+00026e00: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+00026e10: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00026e20: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00026e30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00026e40: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00026e50: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00026e60: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00026e70: 6620 7365 6c66 2e65 7870 6972 655f 7469  f self.expire_ti
+00026e80: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+00026e90: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00026ea0: 6c74 5b27 4578 7069 7265 5469 6d65 275d  lt['ExpireTime']
+00026eb0: 203d 2073 656c 662e 6578 7069 7265 5f74   = self.expire_t
+00026ec0: 696d 650a 2020 2020 2020 2020 6966 2073  ime.        if s
+00026ed0: 656c 662e 7461 7267 6574 5f69 6420 6973  elf.target_id is
+00026ee0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00026ef0: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
+00026f00: 6172 6765 7449 6427 5d20 3d20 7365 6c66  argetId'] = self
+00026f10: 2e74 6172 6765 745f 6964 0a20 2020 2020  .target_id.     
+00026f20: 2020 2069 6620 7365 6c66 2e74 6172 6765     if self.targe
+00026f30: 745f 7479 7065 2069 7320 6e6f 7420 4e6f  t_type is not No
+00026f40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00026f50: 7265 7375 6c74 5b27 5461 7267 6574 5479  result['TargetTy
+00026f60: 7065 275d 203d 2073 656c 662e 7461 7267  pe'] = self.targ
+00026f70: 6574 5f74 7970 650a 2020 2020 2020 2020  et_type.        
+00026f80: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00026f90: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00026fa0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+00026fb0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+00026fc0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+00026fd0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00026fe0: 2745 7870 6972 6554 696d 6527 2920 6973  'ExpireTime') is
+00026ff0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00027000: 2020 2020 2020 2073 656c 662e 6578 7069         self.expi
+00027010: 7265 5f74 696d 6520 3d20 6d2e 6765 7428  re_time = m.get(
+00027020: 2745 7870 6972 6554 696d 6527 290a 2020  'ExpireTime').  
+00027030: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00027040: 5461 7267 6574 4964 2729 2069 7320 6e6f  TargetId') is no
+00027050: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00027060: 2020 2020 7365 6c66 2e74 6172 6765 745f      self.target_
+00027070: 6964 203d 206d 2e67 6574 2827 5461 7267  id = m.get('Targ
+00027080: 6574 4964 2729 0a20 2020 2020 2020 2069  etId').        i
+00027090: 6620 6d2e 6765 7428 2754 6172 6765 7454  f m.get('TargetT
+000270a0: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
+000270b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000270c0: 656c 662e 7461 7267 6574 5f74 7970 6520  elf.target_type 
+000270d0: 3d20 6d2e 6765 7428 2754 6172 6765 7454  = m.get('TargetT
+000270e0: 7970 6527 290a 2020 2020 2020 2020 7265  ype').        re
+000270f0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00027100: 7320 4765 7454 6f6b 656e 5265 7370 6f6e  s GetTokenRespon
+00027110: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
+00027120: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00027130: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00027140: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
+00027150: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
+00027160: 2c0a 2020 2020 2020 2020 746f 6b65 6e3a  ,.        token:
+00027170: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00027180: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+00027190: 2e72 6571 7565 7374 5f69 6420 3d20 7265  .request_id = re
+000271a0: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+000271b0: 2073 656c 662e 746f 6b65 6e20 3d20 746f   self.token = to
+000271c0: 6b65 6e0a 0a20 2020 2064 6566 2076 616c  ken..    def val
+000271d0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000271e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000271f0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00027200: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00027210: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+00027220: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00027230: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00027240: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00027250: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00027260: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00027270: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00027280: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
+00027290: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000272a0: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
+000272b0: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
+000272c0: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+000272d0: 2069 6620 7365 6c66 2e74 6f6b 656e 2069   if self.token i
+000272e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000272f0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00027300: 546f 6b65 6e27 5d20 3d20 7365 6c66 2e74  Token'] = self.t
+00027310: 6f6b 656e 0a20 2020 2020 2020 2072 6574  oken.        ret
+00027320: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00027330: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00027340: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+00027350: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00027360: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00027370: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+00027380: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
+00027390: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000273a0: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+000273b0: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
+000273c0: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
+000273d0: 6966 206d 2e67 6574 2827 546f 6b65 6e27  if m.get('Token'
+000273e0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000273f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00027400: 746f 6b65 6e20 3d20 6d2e 6765 7428 2754  token = m.get('T
+00027410: 6f6b 656e 2729 0a20 2020 2020 2020 2072  oken').        r
+00027420: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00027430: 7373 2047 6574 546f 6b65 6e52 6573 706f  ss GetTokenRespo
+00027440: 6e73 6528 5465 614d 6f64 656c 293a 0a20  nse(TeaModel):. 
+00027450: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00027460: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00027470: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
+00027480: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
+00027490: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+000274a0: 7461 7475 735f 636f 6465 3a20 696e 7420  tatus_code: int 
+000274b0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+000274c0: 626f 6479 3a20 4765 7454 6f6b 656e 5265  body: GetTokenRe
+000274d0: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
+000274e0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000274f0: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00027500: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
+00027510: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00027520: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
+00027530: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+00027540: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
+00027550: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+00027560: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
+00027570: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00027580: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
+00027590: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+000275a0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+000275b0: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
+000275c0: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
+000275d0: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
+000275e0: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+000275f0: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
+00027600: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
+00027610: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+00027620: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00027630: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+00027640: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+00027650: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00027660: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+00027670: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00027680: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00027690: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000276a0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+000276b0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000276c0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000276d0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+000276e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000276f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00027700: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+00027710: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+00027720: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+00027730: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00027740: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00027750: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+00027760: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+00027770: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00027780: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00027790: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000277a0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+000277b0: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+000277c0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+000277d0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000277e0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000277f0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00027800: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00027810: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00027820: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00027830: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+00027840: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00027850: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+00027860: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+00027870: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+00027880: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00027890: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+000278a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000278b0: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+000278c0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+000278d0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+000278e0: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+000278f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00027900: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00027910: 203d 2047 6574 546f 6b65 6e52 6573 706f   = GetTokenRespo
+00027920: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
+00027930: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+00027940: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+00027950: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+00027960: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00027970: 7365 6c66 0a0a 0a63 6c61 7373 2047 6574  self...class Get
+00027980: 5765 6254 6572 6d69 6e61 6c52 6571 7565  WebTerminalReque
+00027990: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
+000279a0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+000279b0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000279c0: 2020 2020 2020 706f 645f 7569 643a 2073        pod_uid: s
+000279d0: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+000279e0: 3a0a 2020 2020 2020 2020 2320 506f 6420  :.        # Pod 
+000279f0: 5549 44e3 8082 0a20 2020 2020 2020 2073  UID....        s
+00027a00: 656c 662e 706f 645f 7569 6420 3d20 706f  elf.pod_uid = po
+00027a10: 645f 7569 640a 0a20 2020 2064 6566 2076  d_uid..    def v
+00027a20: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+00027a30: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00027a40: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+00027a50: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+00027a60: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+00027a70: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+00027a80: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+00027a90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00027aa0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00027ab0: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00027ac0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00027ad0: 2e70 6f64 5f75 6964 2069 7320 6e6f 7420  .pod_uid is not 
+00027ae0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00027af0: 2020 7265 7375 6c74 5b27 506f 6455 6964    result['PodUid
+00027b00: 275d 203d 2073 656c 662e 706f 645f 7569  '] = self.pod_ui
+00027b10: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+00027b20: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00027b30: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00027b40: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+00027b50: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00027b60: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00027b70: 2069 6620 6d2e 6765 7428 2750 6f64 5569   if m.get('PodUi
+00027b80: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00027b90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00027ba0: 662e 706f 645f 7569 6420 3d20 6d2e 6765  f.pod_uid = m.ge
+00027bb0: 7428 2750 6f64 5569 6427 290a 2020 2020  t('PodUid').    
+00027bc0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00027bd0: 0a0a 636c 6173 7320 4765 7457 6562 5465  ..class GetWebTe
+00027be0: 726d 696e 616c 5265 7370 6f6e 7365 426f  rminalResponseBo
+00027bf0: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
+00027c00: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00027c10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00027c20: 2020 2020 2020 7265 7175 6573 745f 6964        request_id
+00027c30: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00027c40: 2020 2020 2020 7765 625f 7465 726d 696e        web_termin
+00027c50: 616c 5f75 726c 3a20 7374 7220 3d20 4e6f  al_url: str = No
+00027c60: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+00027c70: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+00027c80: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
+00027c90: 2020 2020 2020 2020 7365 6c66 2e77 6562          self.web
+00027ca0: 5f74 6572 6d69 6e61 6c5f 7572 6c20 3d20  _terminal_url = 
+00027cb0: 7765 625f 7465 726d 696e 616c 5f75 726c  web_terminal_url
+00027cc0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00027cd0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00027ce0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00027cf0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+00027d00: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+00027d10: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+00027d20: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00027d30: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00027d40: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00027d50: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00027d60: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00027d70: 2020 2020 6966 2073 656c 662e 7265 7175      if self.requ
+00027d80: 6573 745f 6964 2069 7320 6e6f 7420 4e6f  est_id is not No
+00027d90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00027da0: 7265 7375 6c74 5b27 5265 7175 6573 7449  result['RequestI
+00027db0: 6427 5d20 3d20 7365 6c66 2e72 6571 7565  d'] = self.reque
+00027dc0: 7374 5f69 640a 2020 2020 2020 2020 6966  st_id.        if
+00027dd0: 2073 656c 662e 7765 625f 7465 726d 696e   self.web_termin
+00027de0: 616c 5f75 726c 2069 7320 6e6f 7420 4e6f  al_url is not No
+00027df0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00027e00: 7265 7375 6c74 5b27 5765 6254 6572 6d69  result['WebTermi
+00027e10: 6e61 6c55 726c 275d 203d 2073 656c 662e  nalUrl'] = self.
+00027e20: 7765 625f 7465 726d 696e 616c 5f75 726c  web_terminal_url
+00027e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00027e40: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00027e50: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00027e60: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+00027e70: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+00027e80: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00027e90: 6966 206d 2e67 6574 2827 5265 7175 6573  if m.get('Reques
+00027ea0: 7449 6427 2920 6973 206e 6f74 204e 6f6e  tId') is not Non
+00027eb0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00027ec0: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+00027ed0: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+00027ee0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+00027ef0: 2e67 6574 2827 5765 6254 6572 6d69 6e61  .get('WebTermina
+00027f00: 6c55 726c 2729 2069 7320 6e6f 7420 4e6f  lUrl') is not No
+00027f10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00027f20: 7365 6c66 2e77 6562 5f74 6572 6d69 6e61  self.web_termina
+00027f30: 6c5f 7572 6c20 3d20 6d2e 6765 7428 2757  l_url = m.get('W
+00027f40: 6562 5465 726d 696e 616c 5572 6c27 290a  ebTerminalUrl').
+00027f50: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00027f60: 656c 660a 0a0a 636c 6173 7320 4765 7457  elf...class GetW
+00027f70: 6562 5465 726d 696e 616c 5265 7370 6f6e  ebTerminalRespon
+00027f80: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+00027f90: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00027fa0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00027fb0: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
+00027fc0: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
+00027fd0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+00027fe0: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
+00027ff0: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
+00028000: 6f64 793a 2047 6574 5765 6254 6572 6d69  ody: GetWebTermi
+00028010: 6e61 6c52 6573 706f 6e73 6542 6f64 7920  nalResponseBody 
+00028020: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+00028030: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+00028040: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
+00028050: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00028060: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
+00028070: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
+00028080: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
+00028090: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+000280a0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+000280b0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+000280c0: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
+000280d0: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
+000280e0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+000280f0: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+00028100: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
+00028110: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
+00028120: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+00028130: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+00028140: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
+00028150: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00028160: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+00028170: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+00028180: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+00028190: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000281a0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000281b0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+000281c0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+000281d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000281e0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+000281f0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00028200: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00028210: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+00028220: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+00028230: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00028240: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+00028250: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+00028260: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00028270: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+00028280: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00028290: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+000282a0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+000282b0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+000282c0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+000282d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000282e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000282f0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+00028300: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+00028310: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00028320: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00028330: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+00028340: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+00028350: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+00028360: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00028370: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+00028380: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00028390: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+000283a0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+000283b0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+000283c0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+000283d0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+000283e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000283f0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+00028400: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+00028410: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+00028420: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+00028430: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00028440: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+00028450: 6d6f 6465 6c20 3d20 4765 7457 6562 5465  model = GetWebTe
+00028460: 726d 696e 616c 5265 7370 6f6e 7365 426f  rminalResponseBo
+00028470: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+00028480: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+00028490: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+000284a0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+000284b0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000284c0: 0a0a 636c 6173 7320 4c69 7374 4563 7353  ..class ListEcsS
+000284d0: 7065 6373 5265 7175 6573 7428 5465 614d  pecsRequest(TeaM
+000284e0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+000284f0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00028500: 2073 656c 662c 0a20 2020 2020 2020 2061   self,.        a
+00028510: 6363 656c 6572 6174 6f72 5f74 7970 653a  ccelerator_type:
+00028520: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00028530: 2020 2020 206f 7264 6572 3a20 7374 7220       order: str 
+00028540: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00028550: 7061 6765 5f6e 756d 6265 723a 2069 6e74  page_number: int
+00028560: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00028570: 2070 6167 655f 7369 7a65 3a20 696e 7420   page_size: int 
+00028580: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00028590: 736f 7274 5f62 793a 2073 7472 203d 204e  sort_by: str = N
+000285a0: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+000285b0: 2020 2020 7365 6c66 2e61 6363 656c 6572      self.acceler
+000285c0: 6174 6f72 5f74 7970 6520 3d20 6163 6365  ator_type = acce
+000285d0: 6c65 7261 746f 725f 7479 7065 0a20 2020  lerator_type.   
+000285e0: 2020 2020 2073 656c 662e 6f72 6465 7220       self.order 
+000285f0: 3d20 6f72 6465 720a 2020 2020 2020 2020  = order.        
+00028600: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
+00028610: 203d 2070 6167 655f 6e75 6d62 6572 0a20   = page_number. 
+00028620: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
+00028630: 5f73 697a 6520 3d20 7061 6765 5f73 697a  _size = page_siz
+00028640: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
+00028650: 6f72 745f 6279 203d 2073 6f72 745f 6279  ort_by = sort_by
+00028660: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00028670: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00028680: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00028690: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+000286a0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+000286b0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+000286c0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+000286d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000286e0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+000286f0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00028700: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00028710: 2020 2020 6966 2073 656c 662e 6163 6365      if self.acce
+00028720: 6c65 7261 746f 725f 7479 7065 2069 7320  lerator_type is 
+00028730: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00028740: 2020 2020 2020 7265 7375 6c74 5b27 4163        result['Ac
+00028750: 6365 6c65 7261 746f 7254 7970 6527 5d20  celeratorType'] 
+00028760: 3d20 7365 6c66 2e61 6363 656c 6572 6174  = self.accelerat
+00028770: 6f72 5f74 7970 650a 2020 2020 2020 2020  or_type.        
+00028780: 6966 2073 656c 662e 6f72 6465 7220 6973  if self.order is
+00028790: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000287a0: 2020 2020 2020 2072 6573 756c 745b 274f         result['O
+000287b0: 7264 6572 275d 203d 2073 656c 662e 6f72  rder'] = self.or
+000287c0: 6465 720a 2020 2020 2020 2020 6966 2073  der.        if s
+000287d0: 656c 662e 7061 6765 5f6e 756d 6265 7220  elf.page_number 
+000287e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000287f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00028800: 2750 6167 654e 756d 6265 7227 5d20 3d20  'PageNumber'] = 
+00028810: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
+00028820: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00028830: 2e70 6167 655f 7369 7a65 2069 7320 6e6f  .page_size is no
+00028840: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00028850: 2020 2020 7265 7375 6c74 5b27 5061 6765      result['Page
+00028860: 5369 7a65 275d 203d 2073 656c 662e 7061  Size'] = self.pa
+00028870: 6765 5f73 697a 650a 2020 2020 2020 2020  ge_size.        
+00028880: 6966 2073 656c 662e 736f 7274 5f62 7920  if self.sort_by 
+00028890: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000288a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+000288b0: 2753 6f72 7442 7927 5d20 3d20 7365 6c66  'SortBy'] = self
+000288c0: 2e73 6f72 745f 6279 0a20 2020 2020 2020  .sort_by.       
+000288d0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+000288e0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+000288f0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00028900: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00028910: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+00028920: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00028930: 2827 4163 6365 6c65 7261 746f 7254 7970  ('AcceleratorTyp
+00028940: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00028950: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00028960: 662e 6163 6365 6c65 7261 746f 725f 7479  f.accelerator_ty
+00028970: 7065 203d 206d 2e67 6574 2827 4163 6365  pe = m.get('Acce
+00028980: 6c65 7261 746f 7254 7970 6527 290a 2020  leratorType').  
+00028990: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000289a0: 4f72 6465 7227 2920 6973 206e 6f74 204e  Order') is not N
+000289b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000289c0: 2073 656c 662e 6f72 6465 7220 3d20 6d2e   self.order = m.
+000289d0: 6765 7428 274f 7264 6572 2729 0a20 2020  get('Order').   
+000289e0: 2020 2020 2069 6620 6d2e 6765 7428 2750       if m.get('P
+000289f0: 6167 654e 756d 6265 7227 2920 6973 206e  ageNumber') is n
+00028a00: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00028a10: 2020 2020 2073 656c 662e 7061 6765 5f6e       self.page_n
+00028a20: 756d 6265 7220 3d20 6d2e 6765 7428 2750  umber = m.get('P
+00028a30: 6167 654e 756d 6265 7227 290a 2020 2020  ageNumber').    
+00028a40: 2020 2020 6966 206d 2e67 6574 2827 5061      if m.get('Pa
+00028a50: 6765 5369 7a65 2729 2069 7320 6e6f 7420  geSize') is not 
+00028a60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00028a70: 2020 7365 6c66 2e70 6167 655f 7369 7a65    self.page_size
+00028a80: 203d 206d 2e67 6574 2827 5061 6765 5369   = m.get('PageSi
+00028a90: 7a65 2729 0a20 2020 2020 2020 2069 6620  ze').        if 
+00028aa0: 6d2e 6765 7428 2753 6f72 7442 7927 2920  m.get('SortBy') 
+00028ab0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00028ac0: 2020 2020 2020 2020 2073 656c 662e 736f           self.so
+00028ad0: 7274 5f62 7920 3d20 6d2e 6765 7428 2753  rt_by = m.get('S
+00028ae0: 6f72 7442 7927 290a 2020 2020 2020 2020  ortBy').        
+00028af0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00028b00: 6173 7320 4c69 7374 4563 7353 7065 6373  ass ListEcsSpecs
+00028b10: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
+00028b20: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+00028b30: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00028b40: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00028b50: 6563 735f 7370 6563 733a 204c 6973 745b  ecs_specs: List[
+00028b60: 4563 7353 7065 635d 203d 204e 6f6e 652c  EcsSpec] = None,
+00028b70: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+00028b80: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00028b90: 0a20 2020 2020 2020 2074 6f74 616c 5f63  .        total_c
+00028ba0: 6f75 6e74 3a20 696e 7420 3d20 4e6f 6e65  ount: int = None
+00028bb0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00028bc0: 2073 656c 662e 6563 735f 7370 6563 7320   self.ecs_specs 
+00028bd0: 3d20 6563 735f 7370 6563 730a 2020 2020  = ecs_specs.    
+00028be0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+00028bf0: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
+00028c00: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
+00028c10: 7461 6c5f 636f 756e 7420 3d20 746f 7461  tal_count = tota
+00028c20: 6c5f 636f 756e 740a 0a20 2020 2064 6566  l_count..    def
+00028c30: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+00028c40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00028c50: 2e65 6373 5f73 7065 6373 3a0a 2020 2020  .ecs_specs:.    
+00028c60: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
+00028c70: 2073 656c 662e 6563 735f 7370 6563 733a   self.ecs_specs:
+00028c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028c90: 2069 6620 6b3a 0a20 2020 2020 2020 2020   if k:.         
+00028ca0: 2020 2020 2020 2020 2020 206b 2e76 616c             k.val
+00028cb0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+00028cc0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+00028cd0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+00028ce0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+00028cf0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+00028d00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00028d10: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00028d20: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+00028d30: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+00028d40: 2020 2020 2072 6573 756c 745b 2745 6373       result['Ecs
+00028d50: 5370 6563 7327 5d20 3d20 5b5d 0a20 2020  Specs'] = [].   
+00028d60: 2020 2020 2069 6620 7365 6c66 2e65 6373       if self.ecs
+00028d70: 5f73 7065 6373 2069 7320 6e6f 7420 4e6f  _specs is not No
+00028d80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00028d90: 666f 7220 6b20 696e 2073 656c 662e 6563  for k in self.ec
+00028da0: 735f 7370 6563 733a 0a20 2020 2020 2020  s_specs:.       
+00028db0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00028dc0: 2745 6373 5370 6563 7327 5d2e 6170 7065  'EcsSpecs'].appe
+00028dd0: 6e64 286b 2e74 6f5f 6d61 7028 2920 6966  nd(k.to_map() if
+00028de0: 206b 2065 6c73 6520 4e6f 6e65 290a 2020   k else None).  
+00028df0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+00028e00: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
+00028e10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00028e20: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
+00028e30: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
+00028e40: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
+00028e50: 6966 2073 656c 662e 746f 7461 6c5f 636f  if self.total_co
+00028e60: 756e 7420 6973 206e 6f74 204e 6f6e 653a  unt is not None:
+00028e70: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00028e80: 756c 745b 2754 6f74 616c 436f 756e 7427  ult['TotalCount'
+00028e90: 5d20 3d20 7365 6c66 2e74 6f74 616c 5f63  ] = self.total_c
+00028ea0: 6f75 6e74 0a20 2020 2020 2020 2072 6574  ount.        ret
+00028eb0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00028ec0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00028ed0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+00028ee0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00028ef0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00028f00: 2020 2020 7365 6c66 2e65 6373 5f73 7065      self.ecs_spe
+00028f10: 6373 203d 205b 5d0a 2020 2020 2020 2020  cs = [].        
+00028f20: 6966 206d 2e67 6574 2827 4563 7353 7065  if m.get('EcsSpe
+00028f30: 6373 2729 2069 7320 6e6f 7420 4e6f 6e65  cs') is not None
+00028f40: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00028f50: 7220 6b20 696e 206d 2e67 6574 2827 4563  r k in m.get('Ec
+00028f60: 7353 7065 6373 2729 3a0a 2020 2020 2020  sSpecs'):.      
+00028f70: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+00028f80: 6f64 656c 203d 2045 6373 5370 6563 2829  odel = EcsSpec()
+00028f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00028fa0: 2073 656c 662e 6563 735f 7370 6563 732e   self.ecs_specs.
+00028fb0: 6170 7065 6e64 2874 656d 705f 6d6f 6465  append(temp_mode
+00028fc0: 6c2e 6672 6f6d 5f6d 6170 286b 2929 0a20  l.from_map(k)). 
+00028fd0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00028fe0: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
+00028ff0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00029000: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+00029010: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
+00029020: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
+00029030: 2020 2069 6620 6d2e 6765 7428 2754 6f74     if m.get('Tot
+00029040: 616c 436f 756e 7427 2920 6973 206e 6f74  alCount') is not
+00029050: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00029060: 2020 2073 656c 662e 746f 7461 6c5f 636f     self.total_co
+00029070: 756e 7420 3d20 6d2e 6765 7428 2754 6f74  unt = m.get('Tot
+00029080: 616c 436f 756e 7427 290a 2020 2020 2020  alCount').      
+00029090: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+000290a0: 636c 6173 7320 4c69 7374 4563 7353 7065  class ListEcsSpe
+000290b0: 6373 5265 7370 6f6e 7365 2854 6561 4d6f  csResponse(TeaMo
+000290c0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+000290d0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000290e0: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+000290f0: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+00029100: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+00029110: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+00029120: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+00029130: 2020 2020 2020 2062 6f64 793a 204c 6973         body: Lis
+00029140: 7445 6373 5370 6563 7352 6573 706f 6e73  tEcsSpecsRespons
+00029150: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
+00029160: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00029170: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+00029180: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+00029190: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+000291a0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+000291b0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+000291c0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+000291d0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+000291e0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+000291f0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+00029200: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
+00029210: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
+00029220: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00029230: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
+00029240: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
+00029250: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
+00029260: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+00029270: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
+00029280: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
+00029290: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
+000292a0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000292b0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
+000292c0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+000292d0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+000292e0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+000292f0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+00029300: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+00029310: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00029320: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+00029330: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+00029340: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+00029350: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+00029360: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00029370: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+00029380: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+00029390: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+000293a0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+000293b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000293c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000293d0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+000293e0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000293f0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+00029400: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+00029410: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00029420: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+00029430: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+00029440: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+00029450: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00029460: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00029470: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+00029480: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+00029490: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+000294a0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
+000294b0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
+000294c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000294d0: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
+000294e0: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
+000294f0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00029500: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
+00029510: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00029520: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00029530: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
+00029540: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
+00029550: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00029560: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+00029570: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00029580: 2074 656d 705f 6d6f 6465 6c20 3d20 4c69   temp_model = Li
+00029590: 7374 4563 7353 7065 6373 5265 7370 6f6e  stEcsSpecsRespon
+000295a0: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
+000295b0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+000295c0: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+000295d0: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+000295e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000295f0: 656c 660a 0a0a 636c 6173 7320 4c69 7374  elf...class List
+00029600: 4a6f 6273 5265 7175 6573 7428 5465 614d  JobsRequest(TeaM
+00029610: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+00029620: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00029630: 2073 656c 662c 0a20 2020 2020 2020 2062   self,.        b
+00029640: 7573 696e 6573 735f 7573 6572 5f69 643a  usiness_user_id:
+00029650: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00029660: 2020 2020 2063 616c 6c65 723a 2073 7472       caller: str
+00029670: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00029680: 2064 6973 706c 6179 5f6e 616d 653a 2073   display_name: s
+00029690: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000296a0: 2020 2065 6e64 5f74 696d 653a 2073 7472     end_time: str
+000296b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000296c0: 2066 726f 6d5f 616c 6c5f 776f 726b 7370   from_all_worksp
+000296d0: 6163 6573 3a20 626f 6f6c 203d 204e 6f6e  aces: bool = Non
+000296e0: 652c 0a20 2020 2020 2020 206a 6f62 5f69  e,.        job_i
+000296f0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+00029700: 2020 2020 2020 206a 6f62 5f74 7970 653a         job_type:
+00029710: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00029720: 2020 2020 206f 7264 6572 3a20 7374 7220       order: str 
+00029730: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00029740: 7061 6765 5f6e 756d 6265 723a 2069 6e74  page_number: int
+00029750: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00029760: 2070 6167 655f 7369 7a65 3a20 696e 7420   page_size: int 
+00029770: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00029780: 7069 7065 6c69 6e65 5f69 643a 2073 7472  pipeline_id: str
+00029790: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000297a0: 2072 6573 6f75 7263 655f 6964 3a20 7374   resource_id: st
+000297b0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+000297c0: 2020 7368 6f77 5f6f 776e 3a20 626f 6f6c    show_own: bool
+000297d0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000297e0: 2073 6f72 745f 6279 3a20 7374 7220 3d20   sort_by: str = 
+000297f0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+00029800: 6172 745f 7469 6d65 3a20 7374 7220 3d20  art_time: str = 
+00029810: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+00029820: 6174 7573 3a20 7374 7220 3d20 4e6f 6e65  atus: str = None
+00029830: 2c0a 2020 2020 2020 2020 7461 6773 3a20  ,.        tags: 
+00029840: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
+00029850: 204e 6f6e 652c 0a20 2020 2020 2020 2077   None,.        w
+00029860: 6f72 6b73 7061 6365 5f69 643a 2073 7472  orkspace_id: str
+00029870: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+00029880: 2020 2020 2020 2020 7365 6c66 2e62 7573          self.bus
+00029890: 696e 6573 735f 7573 6572 5f69 6420 3d20  iness_user_id = 
+000298a0: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
+000298b0: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
+000298c0: 6c6c 6572 203d 2063 616c 6c65 720a 2020  ller = caller.  
+000298d0: 2020 2020 2020 7365 6c66 2e64 6973 706c        self.displ
+000298e0: 6179 5f6e 616d 6520 3d20 6469 7370 6c61  ay_name = displa
+000298f0: 795f 6e61 6d65 0a20 2020 2020 2020 2073  y_name.        s
+00029900: 656c 662e 656e 645f 7469 6d65 203d 2065  elf.end_time = e
+00029910: 6e64 5f74 696d 650a 2020 2020 2020 2020  nd_time.        
+00029920: 7365 6c66 2e66 726f 6d5f 616c 6c5f 776f  self.from_all_wo
+00029930: 726b 7370 6163 6573 203d 2066 726f 6d5f  rkspaces = from_
+00029940: 616c 6c5f 776f 726b 7370 6163 6573 0a20  all_workspaces. 
+00029950: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
+00029960: 6964 203d 206a 6f62 5f69 640a 2020 2020  id = job_id.    
+00029970: 2020 2020 7365 6c66 2e6a 6f62 5f74 7970      self.job_typ
+00029980: 6520 3d20 6a6f 625f 7479 7065 0a20 2020  e = job_type.   
+00029990: 2020 2020 2073 656c 662e 6f72 6465 7220       self.order 
+000299a0: 3d20 6f72 6465 720a 2020 2020 2020 2020  = order.        
+000299b0: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
+000299c0: 203d 2070 6167 655f 6e75 6d62 6572 0a20   = page_number. 
+000299d0: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
+000299e0: 5f73 697a 6520 3d20 7061 6765 5f73 697a  _size = page_siz
+000299f0: 650a 2020 2020 2020 2020 7365 6c66 2e70  e.        self.p
+00029a00: 6970 656c 696e 655f 6964 203d 2070 6970  ipeline_id = pip
+00029a10: 656c 696e 655f 6964 0a20 2020 2020 2020  eline_id.       
+00029a20: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
+00029a30: 6420 3d20 7265 736f 7572 6365 5f69 640a  d = resource_id.
+00029a40: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
+00029a50: 775f 6f77 6e20 3d20 7368 6f77 5f6f 776e  w_own = show_own
+00029a60: 0a20 2020 2020 2020 2073 656c 662e 736f  .        self.so
+00029a70: 7274 5f62 7920 3d20 736f 7274 5f62 790a  rt_by = sort_by.
+00029a80: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00029a90: 7274 5f74 696d 6520 3d20 7374 6172 745f  rt_time = start_
+00029aa0: 7469 6d65 0a20 2020 2020 2020 2073 656c  time.        sel
+00029ab0: 662e 7374 6174 7573 203d 2073 7461 7475  f.status = statu
+00029ac0: 730a 2020 2020 2020 2020 7365 6c66 2e74  s.        self.t
+00029ad0: 6167 7320 3d20 7461 6773 0a20 2020 2020  ags = tags.     
+00029ae0: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
+00029af0: 655f 6964 203d 2077 6f72 6b73 7061 6365  e_id = workspace
+00029b00: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
+00029b10: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00029b20: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00029b30: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00029b40: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+00029b50: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+00029b60: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00029b70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00029b80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00029b90: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00029ba0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00029bb0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00029bc0: 7573 696e 6573 735f 7573 6572 5f69 6420  usiness_user_id 
+00029bd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00029be0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00029bf0: 2742 7573 696e 6573 7355 7365 7249 6427  'BusinessUserId'
+00029c00: 5d20 3d20 7365 6c66 2e62 7573 696e 6573  ] = self.busines
+00029c10: 735f 7573 6572 5f69 640a 2020 2020 2020  s_user_id.      
+00029c20: 2020 6966 2073 656c 662e 6361 6c6c 6572    if self.caller
+00029c30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00029c40: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00029c50: 5b27 4361 6c6c 6572 275d 203d 2073 656c  ['Caller'] = sel
+00029c60: 662e 6361 6c6c 6572 0a20 2020 2020 2020  f.caller.       
+00029c70: 2069 6620 7365 6c66 2e64 6973 706c 6179   if self.display
+00029c80: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
+00029c90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00029ca0: 6573 756c 745b 2744 6973 706c 6179 4e61  esult['DisplayNa
+00029cb0: 6d65 275d 203d 2073 656c 662e 6469 7370  me'] = self.disp
+00029cc0: 6c61 795f 6e61 6d65 0a20 2020 2020 2020  lay_name.       
+00029cd0: 2069 6620 7365 6c66 2e65 6e64 5f74 696d   if self.end_tim
+00029ce0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00029cf0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00029d00: 745b 2745 6e64 5469 6d65 275d 203d 2073  t['EndTime'] = s
+00029d10: 656c 662e 656e 645f 7469 6d65 0a20 2020  elf.end_time.   
+00029d20: 2020 2020 2069 6620 7365 6c66 2e66 726f       if self.fro
+00029d30: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
+00029d40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00029d50: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00029d60: 5b27 4672 6f6d 416c 6c57 6f72 6b73 7061  ['FromAllWorkspa
+00029d70: 6365 7327 5d20 3d20 7365 6c66 2e66 726f  ces'] = self.fro
+00029d80: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
+00029d90: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00029da0: 2e6a 6f62 5f69 6420 6973 206e 6f74 204e  .job_id is not N
+00029db0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00029dc0: 2072 6573 756c 745b 274a 6f62 4964 275d   result['JobId']
+00029dd0: 203d 2073 656c 662e 6a6f 625f 6964 0a20   = self.job_id. 
+00029de0: 2020 2020 2020 2069 6620 7365 6c66 2e6a         if self.j
+00029df0: 6f62 5f74 7970 6520 6973 206e 6f74 204e  ob_type is not N
+00029e00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00029e10: 2072 6573 756c 745b 274a 6f62 5479 7065   result['JobType
+00029e20: 275d 203d 2073 656c 662e 6a6f 625f 7479  '] = self.job_ty
+00029e30: 7065 0a20 2020 2020 2020 2069 6620 7365  pe.        if se
+00029e40: 6c66 2e6f 7264 6572 2069 7320 6e6f 7420  lf.order is not 
+00029e50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00029e60: 2020 7265 7375 6c74 5b27 4f72 6465 7227    result['Order'
+00029e70: 5d20 3d20 7365 6c66 2e6f 7264 6572 0a20  ] = self.order. 
+00029e80: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00029e90: 6167 655f 6e75 6d62 6572 2069 7320 6e6f  age_number is no
+00029ea0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00029eb0: 2020 2020 7265 7375 6c74 5b27 5061 6765      result['Page
+00029ec0: 4e75 6d62 6572 275d 203d 2073 656c 662e  Number'] = self.
+00029ed0: 7061 6765 5f6e 756d 6265 720a 2020 2020  page_number.    
+00029ee0: 2020 2020 6966 2073 656c 662e 7061 6765      if self.page
+00029ef0: 5f73 697a 6520 6973 206e 6f74 204e 6f6e  _size is not Non
+00029f00: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00029f10: 6573 756c 745b 2750 6167 6553 697a 6527  esult['PageSize'
+00029f20: 5d20 3d20 7365 6c66 2e70 6167 655f 7369  ] = self.page_si
+00029f30: 7a65 0a20 2020 2020 2020 2069 6620 7365  ze.        if se
+00029f40: 6c66 2e70 6970 656c 696e 655f 6964 2069  lf.pipeline_id i
+00029f50: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00029f60: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00029f70: 5069 7065 6c69 6e65 4964 275d 203d 2073  PipelineId'] = s
+00029f80: 656c 662e 7069 7065 6c69 6e65 5f69 640a  elf.pipeline_id.
+00029f90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00029fa0: 7265 736f 7572 6365 5f69 6420 6973 206e  resource_id is n
+00029fb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00029fc0: 2020 2020 2072 6573 756c 745b 2752 6573       result['Res
+00029fd0: 6f75 7263 6549 6427 5d20 3d20 7365 6c66  ourceId'] = self
+00029fe0: 2e72 6573 6f75 7263 655f 6964 0a20 2020  .resource_id.   
+00029ff0: 2020 2020 2069 6620 7365 6c66 2e73 686f       if self.sho
+0002a000: 775f 6f77 6e20 6973 206e 6f74 204e 6f6e  w_own is not Non
+0002a010: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002a020: 6573 756c 745b 2753 686f 774f 776e 275d  esult['ShowOwn']
+0002a030: 203d 2073 656c 662e 7368 6f77 5f6f 776e   = self.show_own
+0002a040: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002a050: 2e73 6f72 745f 6279 2069 7320 6e6f 7420  .sort_by is not 
+0002a060: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002a070: 2020 7265 7375 6c74 5b27 536f 7274 4279    result['SortBy
+0002a080: 275d 203d 2073 656c 662e 736f 7274 5f62  '] = self.sort_b
+0002a090: 790a 2020 2020 2020 2020 6966 2073 656c  y.        if sel
+0002a0a0: 662e 7374 6172 745f 7469 6d65 2069 7320  f.start_time is 
+0002a0b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002a0c0: 2020 2020 2020 7265 7375 6c74 5b27 5374        result['St
+0002a0d0: 6172 7454 696d 6527 5d20 3d20 7365 6c66  artTime'] = self
+0002a0e0: 2e73 7461 7274 5f74 696d 650a 2020 2020  .start_time.    
+0002a0f0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+0002a100: 7573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  us is not None:.
+0002a110: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002a120: 6c74 5b27 5374 6174 7573 275d 203d 2073  lt['Status'] = s
+0002a130: 656c 662e 7374 6174 7573 0a20 2020 2020  elf.status.     
+0002a140: 2020 2069 6620 7365 6c66 2e74 6167 7320     if self.tags 
+0002a150: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002a160: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002a170: 2754 6167 7327 5d20 3d20 7365 6c66 2e74  'Tags'] = self.t
+0002a180: 6167 730a 2020 2020 2020 2020 6966 2073  ags.        if s
+0002a190: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+0002a1a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a1b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002a1c0: 5b27 576f 726b 7370 6163 6549 6427 5d20  ['WorkspaceId'] 
+0002a1d0: 3d20 7365 6c66 2e77 6f72 6b73 7061 6365  = self.workspace
+0002a1e0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+0002a1f0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0002a200: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0002a210: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+0002a220: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0002a230: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0002a240: 2020 2069 6620 6d2e 6765 7428 2742 7573     if m.get('Bus
+0002a250: 696e 6573 7355 7365 7249 6427 2920 6973  inessUserId') is
+0002a260: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002a270: 2020 2020 2020 2073 656c 662e 6275 7369         self.busi
+0002a280: 6e65 7373 5f75 7365 725f 6964 203d 206d  ness_user_id = m
+0002a290: 2e67 6574 2827 4275 7369 6e65 7373 5573  .get('BusinessUs
+0002a2a0: 6572 4964 2729 0a20 2020 2020 2020 2069  erId').        i
+0002a2b0: 6620 6d2e 6765 7428 2743 616c 6c65 7227  f m.get('Caller'
+0002a2c0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002a2d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002a2e0: 6361 6c6c 6572 203d 206d 2e67 6574 2827  caller = m.get('
+0002a2f0: 4361 6c6c 6572 2729 0a20 2020 2020 2020  Caller').       
+0002a300: 2069 6620 6d2e 6765 7428 2744 6973 706c   if m.get('Displ
+0002a310: 6179 4e61 6d65 2729 2069 7320 6e6f 7420  ayName') is not 
+0002a320: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002a330: 2020 7365 6c66 2e64 6973 706c 6179 5f6e    self.display_n
+0002a340: 616d 6520 3d20 6d2e 6765 7428 2744 6973  ame = m.get('Dis
+0002a350: 706c 6179 4e61 6d65 2729 0a20 2020 2020  playName').     
+0002a360: 2020 2069 6620 6d2e 6765 7428 2745 6e64     if m.get('End
+0002a370: 5469 6d65 2729 2069 7320 6e6f 7420 4e6f  Time') is not No
+0002a380: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002a390: 7365 6c66 2e65 6e64 5f74 696d 6520 3d20  self.end_time = 
+0002a3a0: 6d2e 6765 7428 2745 6e64 5469 6d65 2729  m.get('EndTime')
+0002a3b0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002a3c0: 7428 2746 726f 6d41 6c6c 576f 726b 7370  t('FromAllWorksp
+0002a3d0: 6163 6573 2729 2069 7320 6e6f 7420 4e6f  aces') is not No
+0002a3e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002a3f0: 7365 6c66 2e66 726f 6d5f 616c 6c5f 776f  self.from_all_wo
+0002a400: 726b 7370 6163 6573 203d 206d 2e67 6574  rkspaces = m.get
+0002a410: 2827 4672 6f6d 416c 6c57 6f72 6b73 7061  ('FromAllWorkspa
+0002a420: 6365 7327 290a 2020 2020 2020 2020 6966  ces').        if
+0002a430: 206d 2e67 6574 2827 4a6f 6249 6427 2920   m.get('JobId') 
+0002a440: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002a450: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
+0002a460: 625f 6964 203d 206d 2e67 6574 2827 4a6f  b_id = m.get('Jo
+0002a470: 6249 6427 290a 2020 2020 2020 2020 6966  bId').        if
+0002a480: 206d 2e67 6574 2827 4a6f 6254 7970 6527   m.get('JobType'
+0002a490: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002a4a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002a4b0: 6a6f 625f 7479 7065 203d 206d 2e67 6574  job_type = m.get
+0002a4c0: 2827 4a6f 6254 7970 6527 290a 2020 2020  ('JobType').    
+0002a4d0: 2020 2020 6966 206d 2e67 6574 2827 4f72      if m.get('Or
+0002a4e0: 6465 7227 2920 6973 206e 6f74 204e 6f6e  der') is not Non
+0002a4f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002a500: 656c 662e 6f72 6465 7220 3d20 6d2e 6765  elf.order = m.ge
+0002a510: 7428 274f 7264 6572 2729 0a20 2020 2020  t('Order').     
+0002a520: 2020 2069 6620 6d2e 6765 7428 2750 6167     if m.get('Pag
+0002a530: 654e 756d 6265 7227 2920 6973 206e 6f74  eNumber') is not
+0002a540: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002a550: 2020 2073 656c 662e 7061 6765 5f6e 756d     self.page_num
+0002a560: 6265 7220 3d20 6d2e 6765 7428 2750 6167  ber = m.get('Pag
+0002a570: 654e 756d 6265 7227 290a 2020 2020 2020  eNumber').      
+0002a580: 2020 6966 206d 2e67 6574 2827 5061 6765    if m.get('Page
+0002a590: 5369 7a65 2729 2069 7320 6e6f 7420 4e6f  Size') is not No
+0002a5a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002a5b0: 7365 6c66 2e70 6167 655f 7369 7a65 203d  self.page_size =
+0002a5c0: 206d 2e67 6574 2827 5061 6765 5369 7a65   m.get('PageSize
+0002a5d0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002a5e0: 6765 7428 2750 6970 656c 696e 6549 6427  get('PipelineId'
+0002a5f0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002a600: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002a610: 7069 7065 6c69 6e65 5f69 6420 3d20 6d2e  pipeline_id = m.
+0002a620: 6765 7428 2750 6970 656c 696e 6549 6427  get('PipelineId'
+0002a630: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002a640: 6574 2827 5265 736f 7572 6365 4964 2729  et('ResourceId')
+0002a650: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a660: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0002a670: 6573 6f75 7263 655f 6964 203d 206d 2e67  esource_id = m.g
+0002a680: 6574 2827 5265 736f 7572 6365 4964 2729  et('ResourceId')
+0002a690: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002a6a0: 7428 2753 686f 774f 776e 2729 2069 7320  t('ShowOwn') is 
+0002a6b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002a6c0: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
+0002a6d0: 6f77 6e20 3d20 6d2e 6765 7428 2753 686f  own = m.get('Sho
+0002a6e0: 774f 776e 2729 0a20 2020 2020 2020 2069  wOwn').        i
+0002a6f0: 6620 6d2e 6765 7428 2753 6f72 7442 7927  f m.get('SortBy'
+0002a700: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002a710: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002a720: 736f 7274 5f62 7920 3d20 6d2e 6765 7428  sort_by = m.get(
+0002a730: 2753 6f72 7442 7927 290a 2020 2020 2020  'SortBy').      
+0002a740: 2020 6966 206d 2e67 6574 2827 5374 6172    if m.get('Star
+0002a750: 7454 696d 6527 2920 6973 206e 6f74 204e  tTime') is not N
+0002a760: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002a770: 2073 656c 662e 7374 6172 745f 7469 6d65   self.start_time
+0002a780: 203d 206d 2e67 6574 2827 5374 6172 7454   = m.get('StartT
+0002a790: 696d 6527 290a 2020 2020 2020 2020 6966  ime').        if
+0002a7a0: 206d 2e67 6574 2827 5374 6174 7573 2729   m.get('Status')
+0002a7b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a7c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0002a7d0: 7461 7475 7320 3d20 6d2e 6765 7428 2753  tatus = m.get('S
+0002a7e0: 7461 7475 7327 290a 2020 2020 2020 2020  tatus').        
+0002a7f0: 6966 206d 2e67 6574 2827 5461 6773 2729  if m.get('Tags')
+0002a800: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a810: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0002a820: 6167 7320 3d20 6d2e 6765 7428 2754 6167  ags = m.get('Tag
+0002a830: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+0002a840: 2e67 6574 2827 576f 726b 7370 6163 6549  .get('WorkspaceI
+0002a850: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002a860: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002a870: 662e 776f 726b 7370 6163 655f 6964 203d  f.workspace_id =
+0002a880: 206d 2e67 6574 2827 576f 726b 7370 6163   m.get('Workspac
+0002a890: 6549 6427 290a 2020 2020 2020 2020 7265  eId').        re
+0002a8a0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0002a8b0: 7320 4c69 7374 4a6f 6273 5368 7269 6e6b  s ListJobsShrink
+0002a8c0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+0002a8d0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0002a8e0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0002a8f0: 662c 0a20 2020 2020 2020 2062 7573 696e  f,.        busin
+0002a900: 6573 735f 7573 6572 5f69 643a 2073 7472  ess_user_id: str
+0002a910: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0002a920: 2063 616c 6c65 723a 2073 7472 203d 204e   caller: str = N
+0002a930: 6f6e 652c 0a20 2020 2020 2020 2064 6973  one,.        dis
+0002a940: 706c 6179 5f6e 616d 653a 2073 7472 203d  play_name: str =
+0002a950: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
+0002a960: 6e64 5f74 696d 653a 2073 7472 203d 204e  nd_time: str = N
+0002a970: 6f6e 652c 0a20 2020 2020 2020 2066 726f  one,.        fro
+0002a980: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
+0002a990: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+0002a9a0: 2020 2020 2020 206a 6f62 5f69 643a 2073         job_id: s
+0002a9b0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0002a9c0: 2020 206a 6f62 5f74 7970 653a 2073 7472     job_type: str
+0002a9d0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0002a9e0: 206f 7264 6572 3a20 7374 7220 3d20 4e6f   order: str = No
+0002a9f0: 6e65 2c0a 2020 2020 2020 2020 7061 6765  ne,.        page
+0002aa00: 5f6e 756d 6265 723a 2069 6e74 203d 204e  _number: int = N
+0002aa10: 6f6e 652c 0a20 2020 2020 2020 2070 6167  one,.        pag
+0002aa20: 655f 7369 7a65 3a20 696e 7420 3d20 4e6f  e_size: int = No
+0002aa30: 6e65 2c0a 2020 2020 2020 2020 7069 7065  ne,.        pipe
+0002aa40: 6c69 6e65 5f69 643a 2073 7472 203d 204e  line_id: str = N
+0002aa50: 6f6e 652c 0a20 2020 2020 2020 2072 6573  one,.        res
+0002aa60: 6f75 7263 655f 6964 3a20 7374 7220 3d20  ource_id: str = 
+0002aa70: 4e6f 6e65 2c0a 2020 2020 2020 2020 7368  None,.        sh
+0002aa80: 6f77 5f6f 776e 3a20 626f 6f6c 203d 204e  ow_own: bool = N
+0002aa90: 6f6e 652c 0a20 2020 2020 2020 2073 6f72  one,.        sor
+0002aaa0: 745f 6279 3a20 7374 7220 3d20 4e6f 6e65  t_by: str = None
+0002aab0: 2c0a 2020 2020 2020 2020 7374 6172 745f  ,.        start_
+0002aac0: 7469 6d65 3a20 7374 7220 3d20 4e6f 6e65  time: str = None
+0002aad0: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+0002aae0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0002aaf0: 2020 2020 2020 7461 6773 5f73 6872 696e        tags_shrin
+0002ab00: 6b3a 2073 7472 203d 204e 6f6e 652c 0a20  k: str = None,. 
+0002ab10: 2020 2020 2020 2077 6f72 6b73 7061 6365         workspace
+0002ab20: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+0002ab30: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0002ab40: 7365 6c66 2e62 7573 696e 6573 735f 7573  self.business_us
+0002ab50: 6572 5f69 6420 3d20 6275 7369 6e65 7373  er_id = business
+0002ab60: 5f75 7365 725f 6964 0a20 2020 2020 2020  _user_id.       
+0002ab70: 2073 656c 662e 6361 6c6c 6572 203d 2063   self.caller = c
+0002ab80: 616c 6c65 720a 2020 2020 2020 2020 7365  aller.        se
+0002ab90: 6c66 2e64 6973 706c 6179 5f6e 616d 6520  lf.display_name 
+0002aba0: 3d20 6469 7370 6c61 795f 6e61 6d65 0a20  = display_name. 
+0002abb0: 2020 2020 2020 2073 656c 662e 656e 645f         self.end_
+0002abc0: 7469 6d65 203d 2065 6e64 5f74 696d 650a  time = end_time.
+0002abd0: 2020 2020 2020 2020 7365 6c66 2e66 726f          self.fro
+0002abe0: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
+0002abf0: 203d 2066 726f 6d5f 616c 6c5f 776f 726b   = from_all_work
+0002ac00: 7370 6163 6573 0a20 2020 2020 2020 2073  spaces.        s
+0002ac10: 656c 662e 6a6f 625f 6964 203d 206a 6f62  elf.job_id = job
+0002ac20: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+0002ac30: 2e6a 6f62 5f74 7970 6520 3d20 6a6f 625f  .job_type = job_
+0002ac40: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
+0002ac50: 662e 6f72 6465 7220 3d20 6f72 6465 720a  f.order = order.
+0002ac60: 2020 2020 2020 2020 7365 6c66 2e70 6167          self.pag
+0002ac70: 655f 6e75 6d62 6572 203d 2070 6167 655f  e_number = page_
+0002ac80: 6e75 6d62 6572 0a20 2020 2020 2020 2073  number.        s
+0002ac90: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
+0002aca0: 7061 6765 5f73 697a 650a 2020 2020 2020  page_size.      
+0002acb0: 2020 7365 6c66 2e70 6970 656c 696e 655f    self.pipeline_
+0002acc0: 6964 203d 2070 6970 656c 696e 655f 6964  id = pipeline_id
+0002acd0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+0002ace0: 736f 7572 6365 5f69 6420 3d20 7265 736f  source_id = reso
+0002acf0: 7572 6365 5f69 640a 2020 2020 2020 2020  urce_id.        
+0002ad00: 7365 6c66 2e73 686f 775f 6f77 6e20 3d20  self.show_own = 
+0002ad10: 7368 6f77 5f6f 776e 0a20 2020 2020 2020  show_own.       
+0002ad20: 2073 656c 662e 736f 7274 5f62 7920 3d20   self.sort_by = 
+0002ad30: 736f 7274 5f62 790a 2020 2020 2020 2020  sort_by.        
+0002ad40: 7365 6c66 2e73 7461 7274 5f74 696d 6520  self.start_time 
+0002ad50: 3d20 7374 6172 745f 7469 6d65 0a20 2020  = start_time.   
+0002ad60: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+0002ad70: 203d 2073 7461 7475 730a 2020 2020 2020   = status.      
+0002ad80: 2020 7365 6c66 2e74 6167 735f 7368 7269    self.tags_shri
+0002ad90: 6e6b 203d 2074 6167 735f 7368 7269 6e6b  nk = tags_shrink
+0002ada0: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
+0002adb0: 726b 7370 6163 655f 6964 203d 2077 6f72  rkspace_id = wor
+0002adc0: 6b73 7061 6365 5f69 640a 0a20 2020 2064  kspace_id..    d
+0002add0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0002ade0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+0002adf0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+0002ae00: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+0002ae10: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+0002ae20: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0002ae30: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0002ae40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002ae50: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0002ae60: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0002ae70: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0002ae80: 7365 6c66 2e62 7573 696e 6573 735f 7573  self.business_us
+0002ae90: 6572 5f69 6420 6973 206e 6f74 204e 6f6e  er_id is not Non
+0002aea0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002aeb0: 6573 756c 745b 2742 7573 696e 6573 7355  esult['BusinessU
+0002aec0: 7365 7249 6427 5d20 3d20 7365 6c66 2e62  serId'] = self.b
+0002aed0: 7573 696e 6573 735f 7573 6572 5f69 640a  usiness_user_id.
+0002aee0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002aef0: 6361 6c6c 6572 2069 7320 6e6f 7420 4e6f  caller is not No
+0002af00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002af10: 7265 7375 6c74 5b27 4361 6c6c 6572 275d  result['Caller']
+0002af20: 203d 2073 656c 662e 6361 6c6c 6572 0a20   = self.caller. 
+0002af30: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+0002af40: 6973 706c 6179 5f6e 616d 6520 6973 206e  isplay_name is n
+0002af50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002af60: 2020 2020 2072 6573 756c 745b 2744 6973       result['Dis
+0002af70: 706c 6179 4e61 6d65 275d 203d 2073 656c  playName'] = sel
+0002af80: 662e 6469 7370 6c61 795f 6e61 6d65 0a20  f.display_name. 
+0002af90: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
+0002afa0: 6e64 5f74 696d 6520 6973 206e 6f74 204e  nd_time is not N
+0002afb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002afc0: 2072 6573 756c 745b 2745 6e64 5469 6d65   result['EndTime
+0002afd0: 275d 203d 2073 656c 662e 656e 645f 7469  '] = self.end_ti
+0002afe0: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
+0002aff0: 6c66 2e66 726f 6d5f 616c 6c5f 776f 726b  lf.from_all_work
+0002b000: 7370 6163 6573 2069 7320 6e6f 7420 4e6f  spaces is not No
+0002b010: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002b020: 7265 7375 6c74 5b27 4672 6f6d 416c 6c57  result['FromAllW
+0002b030: 6f72 6b73 7061 6365 7327 5d20 3d20 7365  orkspaces'] = se
+0002b040: 6c66 2e66 726f 6d5f 616c 6c5f 776f 726b  lf.from_all_work
+0002b050: 7370 6163 6573 0a20 2020 2020 2020 2069  spaces.        i
+0002b060: 6620 7365 6c66 2e6a 6f62 5f69 6420 6973  f self.job_id is
+0002b070: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002b080: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
+0002b090: 6f62 4964 275d 203d 2073 656c 662e 6a6f  obId'] = self.jo
+0002b0a0: 625f 6964 0a20 2020 2020 2020 2069 6620  b_id.        if 
+0002b0b0: 7365 6c66 2e6a 6f62 5f74 7970 6520 6973  self.job_type is
+0002b0c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002b0d0: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
+0002b0e0: 6f62 5479 7065 275d 203d 2073 656c 662e  obType'] = self.
+0002b0f0: 6a6f 625f 7479 7065 0a20 2020 2020 2020  job_type.       
+0002b100: 2069 6620 7365 6c66 2e6f 7264 6572 2069   if self.order i
+0002b110: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002b120: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002b130: 4f72 6465 7227 5d20 3d20 7365 6c66 2e6f  Order'] = self.o
+0002b140: 7264 6572 0a20 2020 2020 2020 2069 6620  rder.        if 
+0002b150: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
+0002b160: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002b170: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002b180: 5b27 5061 6765 4e75 6d62 6572 275d 203d  ['PageNumber'] =
+0002b190: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
+0002b1a0: 720a 2020 2020 2020 2020 6966 2073 656c  r.        if sel
+0002b1b0: 662e 7061 6765 5f73 697a 6520 6973 206e  f.page_size is n
+0002b1c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002b1d0: 2020 2020 2072 6573 756c 745b 2750 6167       result['Pag
+0002b1e0: 6553 697a 6527 5d20 3d20 7365 6c66 2e70  eSize'] = self.p
+0002b1f0: 6167 655f 7369 7a65 0a20 2020 2020 2020  age_size.       
+0002b200: 2069 6620 7365 6c66 2e70 6970 656c 696e   if self.pipelin
+0002b210: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+0002b220: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002b230: 7375 6c74 5b27 5069 7065 6c69 6e65 4964  sult['PipelineId
+0002b240: 275d 203d 2073 656c 662e 7069 7065 6c69  '] = self.pipeli
+0002b250: 6e65 5f69 640a 2020 2020 2020 2020 6966  ne_id.        if
+0002b260: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
+0002b270: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+0002b280: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002b290: 745b 2752 6573 6f75 7263 6549 6427 5d20  t['ResourceId'] 
+0002b2a0: 3d20 7365 6c66 2e72 6573 6f75 7263 655f  = self.resource_
+0002b2b0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+0002b2c0: 6c66 2e73 686f 775f 6f77 6e20 6973 206e  lf.show_own is n
+0002b2d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002b2e0: 2020 2020 2072 6573 756c 745b 2753 686f       result['Sho
+0002b2f0: 774f 776e 275d 203d 2073 656c 662e 7368  wOwn'] = self.sh
+0002b300: 6f77 5f6f 776e 0a20 2020 2020 2020 2069  ow_own.        i
+0002b310: 6620 7365 6c66 2e73 6f72 745f 6279 2069  f self.sort_by i
+0002b320: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002b330: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002b340: 536f 7274 4279 275d 203d 2073 656c 662e  SortBy'] = self.
+0002b350: 736f 7274 5f62 790a 2020 2020 2020 2020  sort_by.        
+0002b360: 6966 2073 656c 662e 7374 6172 745f 7469  if self.start_ti
+0002b370: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
+0002b380: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002b390: 6c74 5b27 5374 6172 7454 696d 6527 5d20  lt['StartTime'] 
+0002b3a0: 3d20 7365 6c66 2e73 7461 7274 5f74 696d  = self.start_tim
+0002b3b0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0002b3c0: 662e 7374 6174 7573 2069 7320 6e6f 7420  f.status is not 
+0002b3d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002b3e0: 2020 7265 7375 6c74 5b27 5374 6174 7573    result['Status
+0002b3f0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+0002b400: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002b410: 2e74 6167 735f 7368 7269 6e6b 2069 7320  .tags_shrink is 
+0002b420: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002b430: 2020 2020 2020 7265 7375 6c74 5b27 5461        result['Ta
+0002b440: 6773 275d 203d 2073 656c 662e 7461 6773  gs'] = self.tags
+0002b450: 5f73 6872 696e 6b0a 2020 2020 2020 2020  _shrink.        
+0002b460: 6966 2073 656c 662e 776f 726b 7370 6163  if self.workspac
+0002b470: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+0002b480: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002b490: 7375 6c74 5b27 576f 726b 7370 6163 6549  sult['WorkspaceI
+0002b4a0: 6427 5d20 3d20 7365 6c66 2e77 6f72 6b73  d'] = self.works
+0002b4b0: 7061 6365 5f69 640a 2020 2020 2020 2020  pace_id.        
+0002b4c0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0002b4d0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+0002b4e0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+0002b4f0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0002b500: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0002b510: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002b520: 2742 7573 696e 6573 7355 7365 7249 6427  'BusinessUserId'
+0002b530: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002b540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002b550: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
+0002b560: 203d 206d 2e67 6574 2827 4275 7369 6e65   = m.get('Busine
+0002b570: 7373 5573 6572 4964 2729 0a20 2020 2020  ssUserId').     
+0002b580: 2020 2069 6620 6d2e 6765 7428 2743 616c     if m.get('Cal
+0002b590: 6c65 7227 2920 6973 206e 6f74 204e 6f6e  ler') is not Non
+0002b5a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002b5b0: 656c 662e 6361 6c6c 6572 203d 206d 2e67  elf.caller = m.g
+0002b5c0: 6574 2827 4361 6c6c 6572 2729 0a20 2020  et('Caller').   
+0002b5d0: 2020 2020 2069 6620 6d2e 6765 7428 2744       if m.get('D
+0002b5e0: 6973 706c 6179 4e61 6d65 2729 2069 7320  isplayName') is 
+0002b5f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002b600: 2020 2020 2020 7365 6c66 2e64 6973 706c        self.displ
+0002b610: 6179 5f6e 616d 6520 3d20 6d2e 6765 7428  ay_name = m.get(
+0002b620: 2744 6973 706c 6179 4e61 6d65 2729 0a20  'DisplayName'). 
+0002b630: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002b640: 2745 6e64 5469 6d65 2729 2069 7320 6e6f  'EndTime') is no
+0002b650: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b660: 2020 2020 7365 6c66 2e65 6e64 5f74 696d      self.end_tim
+0002b670: 6520 3d20 6d2e 6765 7428 2745 6e64 5469  e = m.get('EndTi
+0002b680: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
+0002b690: 6d2e 6765 7428 2746 726f 6d41 6c6c 576f  m.get('FromAllWo
+0002b6a0: 726b 7370 6163 6573 2729 2069 7320 6e6f  rkspaces') is no
+0002b6b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b6c0: 2020 2020 7365 6c66 2e66 726f 6d5f 616c      self.from_al
+0002b6d0: 6c5f 776f 726b 7370 6163 6573 203d 206d  l_workspaces = m
+0002b6e0: 2e67 6574 2827 4672 6f6d 416c 6c57 6f72  .get('FromAllWor
+0002b6f0: 6b73 7061 6365 7327 290a 2020 2020 2020  kspaces').      
+0002b700: 2020 6966 206d 2e67 6574 2827 4a6f 6249    if m.get('JobI
+0002b710: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002b720: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002b730: 662e 6a6f 625f 6964 203d 206d 2e67 6574  f.job_id = m.get
+0002b740: 2827 4a6f 6249 6427 290a 2020 2020 2020  ('JobId').      
+0002b750: 2020 6966 206d 2e67 6574 2827 4a6f 6254    if m.get('JobT
+0002b760: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
+0002b770: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002b780: 656c 662e 6a6f 625f 7479 7065 203d 206d  elf.job_type = m
+0002b790: 2e67 6574 2827 4a6f 6254 7970 6527 290a  .get('JobType').
+0002b7a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002b7b0: 2827 4f72 6465 7227 2920 6973 206e 6f74  ('Order') is not
+0002b7c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002b7d0: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
+0002b7e0: 6d2e 6765 7428 274f 7264 6572 2729 0a20  m.get('Order'). 
+0002b7f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002b800: 2750 6167 654e 756d 6265 7227 2920 6973  'PageNumber') is
+0002b810: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002b820: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
+0002b830: 5f6e 756d 6265 7220 3d20 6d2e 6765 7428  _number = m.get(
+0002b840: 2750 6167 654e 756d 6265 7227 290a 2020  'PageNumber').  
+0002b850: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002b860: 5061 6765 5369 7a65 2729 2069 7320 6e6f  PageSize') is no
+0002b870: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b880: 2020 2020 7365 6c66 2e70 6167 655f 7369      self.page_si
+0002b890: 7a65 203d 206d 2e67 6574 2827 5061 6765  ze = m.get('Page
+0002b8a0: 5369 7a65 2729 0a20 2020 2020 2020 2069  Size').        i
+0002b8b0: 6620 6d2e 6765 7428 2750 6970 656c 696e  f m.get('Pipelin
+0002b8c0: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+0002b8d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002b8e0: 656c 662e 7069 7065 6c69 6e65 5f69 6420  elf.pipeline_id 
+0002b8f0: 3d20 6d2e 6765 7428 2750 6970 656c 696e  = m.get('Pipelin
+0002b900: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
+0002b910: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+0002b920: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+0002b930: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002b940: 6c66 2e72 6573 6f75 7263 655f 6964 203d  lf.resource_id =
+0002b950: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
+0002b960: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0002b970: 6d2e 6765 7428 2753 686f 774f 776e 2729  m.get('ShowOwn')
+0002b980: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002b990: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0002b9a0: 686f 775f 6f77 6e20 3d20 6d2e 6765 7428  how_own = m.get(
+0002b9b0: 2753 686f 774f 776e 2729 0a20 2020 2020  'ShowOwn').     
+0002b9c0: 2020 2069 6620 6d2e 6765 7428 2753 6f72     if m.get('Sor
+0002b9d0: 7442 7927 2920 6973 206e 6f74 204e 6f6e  tBy') is not Non
+0002b9e0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002b9f0: 656c 662e 736f 7274 5f62 7920 3d20 6d2e  elf.sort_by = m.
+0002ba00: 6765 7428 2753 6f72 7442 7927 290a 2020  get('SortBy').  
+0002ba10: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002ba20: 5374 6172 7454 696d 6527 2920 6973 206e  StartTime') is n
+0002ba30: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002ba40: 2020 2020 2073 656c 662e 7374 6172 745f       self.start_
+0002ba50: 7469 6d65 203d 206d 2e67 6574 2827 5374  time = m.get('St
+0002ba60: 6172 7454 696d 6527 290a 2020 2020 2020  artTime').      
+0002ba70: 2020 6966 206d 2e67 6574 2827 5374 6174    if m.get('Stat
+0002ba80: 7573 2729 2069 7320 6e6f 7420 4e6f 6e65  us') is not None
+0002ba90: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002baa0: 6c66 2e73 7461 7475 7320 3d20 6d2e 6765  lf.status = m.ge
+0002bab0: 7428 2753 7461 7475 7327 290a 2020 2020  t('Status').    
+0002bac0: 2020 2020 6966 206d 2e67 6574 2827 5461      if m.get('Ta
+0002bad0: 6773 2729 2069 7320 6e6f 7420 4e6f 6e65  gs') is not None
+0002bae0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002baf0: 6c66 2e74 6167 735f 7368 7269 6e6b 203d  lf.tags_shrink =
+0002bb00: 206d 2e67 6574 2827 5461 6773 2729 0a20   m.get('Tags'). 
+0002bb10: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002bb20: 2757 6f72 6b73 7061 6365 4964 2729 2069  'WorkspaceId') i
+0002bb30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002bb40: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+0002bb50: 6b73 7061 6365 5f69 6420 3d20 6d2e 6765  kspace_id = m.ge
+0002bb60: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
+0002bb70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002bb80: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
+0002bb90: 744a 6f62 7352 6573 706f 6e73 6542 6f64  tJobsResponseBod
+0002bba0: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+0002bbb0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+0002bbc0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0002bbd0: 2020 2020 206a 6f62 733a 204c 6973 745b       jobs: List[
+0002bbe0: 4a6f 6249 7465 6d5d 203d 204e 6f6e 652c  JobItem] = None,
+0002bbf0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
+0002bc00: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+0002bc10: 0a20 2020 2020 2020 2074 6f74 616c 5f63  .        total_c
+0002bc20: 6f75 6e74 3a20 696e 7420 3d20 4e6f 6e65  ount: int = None
+0002bc30: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0002bc40: 2073 656c 662e 6a6f 6273 203d 206a 6f62   self.jobs = job
+0002bc50: 730a 2020 2020 2020 2020 7365 6c66 2e72  s.        self.r
+0002bc60: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
+0002bc70: 6573 745f 6964 0a20 2020 2020 2020 2073  est_id.        s
+0002bc80: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
+0002bc90: 3d20 746f 7461 6c5f 636f 756e 740a 0a20  = total_count.. 
+0002bca0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0002bcb0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+0002bcc0: 6620 7365 6c66 2e6a 6f62 733a 0a20 2020  f self.jobs:.   
+0002bcd0: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
+0002bce0: 6e20 7365 6c66 2e6a 6f62 733a 0a20 2020  n self.jobs:.   
+0002bcf0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0002bd00: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+0002bd10: 2020 2020 2020 206b 2e76 616c 6964 6174         k.validat
+0002bd20: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+0002bd30: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+0002bd40: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+0002bd50: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+0002bd60: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+0002bd70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002bd80: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+0002bd90: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0002bda0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+0002bdb0: 2072 6573 756c 745b 274a 6f62 7327 5d20   result['Jobs'] 
+0002bdc0: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
+0002bdd0: 7365 6c66 2e6a 6f62 7320 6973 206e 6f74  self.jobs is not
+0002bde0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002bdf0: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
+0002be00: 2e6a 6f62 733a 0a20 2020 2020 2020 2020  .jobs:.         
+0002be10: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
+0002be20: 6f62 7327 5d2e 6170 7065 6e64 286b 2e74  obs'].append(k.t
+0002be30: 6f5f 6d61 7028 2920 6966 206b 2065 6c73  o_map() if k els
+0002be40: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
+0002be50: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+0002be60: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0002be70: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002be80: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
+0002be90: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
+0002bea0: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+0002beb0: 662e 746f 7461 6c5f 636f 756e 7420 6973  f.total_count is
+0002bec0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002bed0: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
+0002bee0: 6f74 616c 436f 756e 7427 5d20 3d20 7365  otalCount'] = se
+0002bef0: 6c66 2e74 6f74 616c 5f63 6f75 6e74 0a20  lf.total_count. 
+0002bf00: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0002bf10: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0002bf20: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+0002bf30: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+0002bf40: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+0002bf50: 6963 7428 290a 2020 2020 2020 2020 7365  ict().        se
+0002bf60: 6c66 2e6a 6f62 7320 3d20 5b5d 0a20 2020  lf.jobs = [].   
+0002bf70: 2020 2020 2069 6620 6d2e 6765 7428 274a       if m.get('J
+0002bf80: 6f62 7327 2920 6973 206e 6f74 204e 6f6e  obs') is not Non
+0002bf90: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+0002bfa0: 6f72 206b 2069 6e20 6d2e 6765 7428 274a  or k in m.get('J
+0002bfb0: 6f62 7327 293a 0a20 2020 2020 2020 2020  obs'):.         
+0002bfc0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+0002bfd0: 6c20 3d20 4a6f 6249 7465 6d28 290a 2020  l = JobItem().  
+0002bfe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0002bff0: 6c66 2e6a 6f62 732e 6170 7065 6e64 2874  lf.jobs.append(t
+0002c000: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+0002c010: 6170 286b 2929 0a20 2020 2020 2020 2069  ap(k)).        i
+0002c020: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
+0002c030: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+0002c040: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002c050: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+0002c060: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+0002c070: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002c080: 6765 7428 2754 6f74 616c 436f 756e 7427  get('TotalCount'
+0002c090: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002c0a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002c0b0: 746f 7461 6c5f 636f 756e 7420 3d20 6d2e  total_count = m.
+0002c0c0: 6765 7428 2754 6f74 616c 436f 756e 7427  get('TotalCount'
+0002c0d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0002c0e0: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
+0002c0f0: 7374 4a6f 6273 5265 7370 6f6e 7365 2854  stJobsResponse(T
+0002c100: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0002c110: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0002c120: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0002c130: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
+0002c140: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
+0002c150: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+0002c160: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
+0002c170: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+0002c180: 204c 6973 744a 6f62 7352 6573 706f 6e73   ListJobsRespons
+0002c190: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
+0002c1a0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+0002c1b0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+0002c1c0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
+0002c1d0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+0002c1e0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
+0002c1f0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+0002c200: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
+0002c210: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0002c220: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+0002c230: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+0002c240: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
+0002c250: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
+0002c260: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+0002c270: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
+0002c280: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
+0002c290: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
+0002c2a0: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+0002c2b0: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
+0002c2c0: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
+0002c2d0: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
+0002c2e0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+0002c2f0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
+0002c300: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+0002c310: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+0002c320: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+0002c330: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+0002c340: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+0002c350: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002c360: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+0002c370: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+0002c380: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0002c390: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
+0002c3a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002c3b0: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
+0002c3c0: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
+0002c3d0: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
+0002c3e0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0002c3f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002c400: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002c410: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
+0002c420: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+0002c430: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0002c440: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
+0002c450: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002c460: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
+0002c470: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
+0002c480: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
+0002c490: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0002c4a0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0002c4b0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+0002c4c0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0002c4d0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0002c4e0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
+0002c4f0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
+0002c500: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002c510: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
+0002c520: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
+0002c530: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002c540: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
+0002c550: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002c560: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0002c570: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
+0002c580: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
+0002c590: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002c5a0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
+0002c5b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002c5c0: 2074 656d 705f 6d6f 6465 6c20 3d20 4c69   temp_model = Li
+0002c5d0: 7374 4a6f 6273 5265 7370 6f6e 7365 426f  stJobsResponseBo
+0002c5e0: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+0002c5f0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+0002c600: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+0002c610: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+0002c620: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0002c630: 0a0a 636c 6173 7320 4c69 7374 5465 6e73  ..class ListTens
+0002c640: 6f72 626f 6172 6473 5265 7175 6573 7428  orboardsRequest(
+0002c650: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+0002c660: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+0002c670: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0002c680: 2020 2064 6973 706c 6179 5f6e 616d 653a     display_name:
+0002c690: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0002c6a0: 2020 2020 2065 6e64 5f74 696d 653a 2073       end_time: s
+0002c6b0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0002c6c0: 2020 206a 6f62 5f69 643a 2073 7472 203d     job_id: str =
+0002c6d0: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
+0002c6e0: 7264 6572 3a20 7374 7220 3d20 4e6f 6e65  rder: str = None
+0002c6f0: 2c0a 2020 2020 2020 2020 7061 6765 5f6e  ,.        page_n
+0002c700: 756d 6265 723a 2069 6e74 203d 204e 6f6e  umber: int = Non
+0002c710: 652c 0a20 2020 2020 2020 2070 6167 655f  e,.        page_
+0002c720: 7369 7a65 3a20 696e 7420 3d20 4e6f 6e65  size: int = None
+0002c730: 2c0a 2020 2020 2020 2020 736f 7274 5f62  ,.        sort_b
+0002c740: 793a 2073 7472 203d 204e 6f6e 652c 0a20  y: str = None,. 
+0002c750: 2020 2020 2020 2073 6f75 7263 655f 6964         source_id
+0002c760: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0002c770: 2020 2020 2020 736f 7572 6365 5f74 7970        source_typ
+0002c780: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+0002c790: 2020 2020 2020 2073 7461 7274 5f74 696d         start_tim
+0002c7a0: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
+0002c7b0: 2020 2020 2020 2073 7461 7475 733a 2073         status: s
+0002c7c0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0002c7d0: 2020 2074 656e 736f 7262 6f61 7264 5f69     tensorboard_i
+0002c7e0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0002c7f0: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
+0002c800: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
+0002c810: 2020 2020 2077 6f72 6b73 7061 6365 5f69       workspace_i
+0002c820: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0002c830: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+0002c840: 6c66 2e64 6973 706c 6179 5f6e 616d 6520  lf.display_name 
+0002c850: 3d20 6469 7370 6c61 795f 6e61 6d65 0a20  = display_name. 
+0002c860: 2020 2020 2020 2073 656c 662e 656e 645f         self.end_
+0002c870: 7469 6d65 203d 2065 6e64 5f74 696d 650a  time = end_time.
+0002c880: 2020 2020 2020 2020 7365 6c66 2e6a 6f62          self.job
+0002c890: 5f69 6420 3d20 6a6f 625f 6964 0a20 2020  _id = job_id.   
+0002c8a0: 2020 2020 2073 656c 662e 6f72 6465 7220       self.order 
+0002c8b0: 3d20 6f72 6465 720a 2020 2020 2020 2020  = order.        
+0002c8c0: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
+0002c8d0: 203d 2070 6167 655f 6e75 6d62 6572 0a20   = page_number. 
+0002c8e0: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
+0002c8f0: 5f73 697a 6520 3d20 7061 6765 5f73 697a  _size = page_siz
+0002c900: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
+0002c910: 6f72 745f 6279 203d 2073 6f72 745f 6279  ort_by = sort_by
+0002c920: 0a20 2020 2020 2020 2073 656c 662e 736f  .        self.so
+0002c930: 7572 6365 5f69 6420 3d20 736f 7572 6365  urce_id = source
+0002c940: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+0002c950: 2e73 6f75 7263 655f 7479 7065 203d 2073  .source_type = s
+0002c960: 6f75 7263 655f 7479 7065 0a20 2020 2020  ource_type.     
+0002c970: 2020 2073 656c 662e 7374 6172 745f 7469     self.start_ti
+0002c980: 6d65 203d 2073 7461 7274 5f74 696d 650a  me = start_time.
+0002c990: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0002c9a0: 7475 7320 3d20 7374 6174 7573 0a20 2020  tus = status.   
+0002c9b0: 2020 2020 2073 656c 662e 7465 6e73 6f72       self.tensor
+0002c9c0: 626f 6172 645f 6964 203d 2074 656e 736f  board_id = tenso
+0002c9d0: 7262 6f61 7264 5f69 640a 2020 2020 2020  rboard_id.      
+0002c9e0: 2020 7365 6c66 2e76 6572 626f 7365 203d    self.verbose =
+0002c9f0: 2076 6572 626f 7365 0a20 2020 2020 2020   verbose.       
+0002ca00: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
+0002ca10: 6964 203d 2077 6f72 6b73 7061 6365 5f69  id = workspace_i
+0002ca20: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
+0002ca30: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+0002ca40: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+0002ca50: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0002ca60: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0002ca70: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+0002ca80: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0002ca90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002caa0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0002cab0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0002cac0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0002cad0: 2020 2020 2069 6620 7365 6c66 2e64 6973       if self.dis
+0002cae0: 706c 6179 5f6e 616d 6520 6973 206e 6f74  play_name is not
+0002caf0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002cb00: 2020 2072 6573 756c 745b 2744 6973 706c     result['Displ
+0002cb10: 6179 4e61 6d65 275d 203d 2073 656c 662e  ayName'] = self.
+0002cb20: 6469 7370 6c61 795f 6e61 6d65 0a20 2020  display_name.   
+0002cb30: 2020 2020 2069 6620 7365 6c66 2e65 6e64       if self.end
+0002cb40: 5f74 696d 6520 6973 206e 6f74 204e 6f6e  _time is not Non
+0002cb50: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002cb60: 6573 756c 745b 2745 6e64 5469 6d65 275d  esult['EndTime']
+0002cb70: 203d 2073 656c 662e 656e 645f 7469 6d65   = self.end_time
+0002cb80: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002cb90: 2e6a 6f62 5f69 6420 6973 206e 6f74 204e  .job_id is not N
+0002cba0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002cbb0: 2072 6573 756c 745b 274a 6f62 4964 275d   result['JobId']
+0002cbc0: 203d 2073 656c 662e 6a6f 625f 6964 0a20   = self.job_id. 
+0002cbd0: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
+0002cbe0: 7264 6572 2069 7320 6e6f 7420 4e6f 6e65  rder is not None
+0002cbf0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002cc00: 7375 6c74 5b27 4f72 6465 7227 5d20 3d20  sult['Order'] = 
+0002cc10: 7365 6c66 2e6f 7264 6572 0a20 2020 2020  self.order.     
+0002cc20: 2020 2069 6620 7365 6c66 2e70 6167 655f     if self.page_
+0002cc30: 6e75 6d62 6572 2069 7320 6e6f 7420 4e6f  number is not No
+0002cc40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002cc50: 7265 7375 6c74 5b27 5061 6765 4e75 6d62  result['PageNumb
+0002cc60: 6572 275d 203d 2073 656c 662e 7061 6765  er'] = self.page
+0002cc70: 5f6e 756d 6265 720a 2020 2020 2020 2020  _number.        
+0002cc80: 6966 2073 656c 662e 7061 6765 5f73 697a  if self.page_siz
+0002cc90: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+0002cca0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002ccb0: 745b 2750 6167 6553 697a 6527 5d20 3d20  t['PageSize'] = 
+0002ccc0: 7365 6c66 2e70 6167 655f 7369 7a65 0a20  self.page_size. 
+0002ccd0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0002cce0: 6f72 745f 6279 2069 7320 6e6f 7420 4e6f  ort_by is not No
+0002ccf0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002cd00: 7265 7375 6c74 5b27 536f 7274 4279 275d  result['SortBy']
+0002cd10: 203d 2073 656c 662e 736f 7274 5f62 790a   = self.sort_by.
+0002cd20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002cd30: 736f 7572 6365 5f69 6420 6973 206e 6f74  source_id is not
+0002cd40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002cd50: 2020 2072 6573 756c 745b 2753 6f75 7263     result['Sourc
+0002cd60: 6549 6427 5d20 3d20 7365 6c66 2e73 6f75  eId'] = self.sou
+0002cd70: 7263 655f 6964 0a20 2020 2020 2020 2069  rce_id.        i
+0002cd80: 6620 7365 6c66 2e73 6f75 7263 655f 7479  f self.source_ty
+0002cd90: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
+0002cda0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002cdb0: 6c74 5b27 536f 7572 6365 5479 7065 275d  lt['SourceType']
+0002cdc0: 203d 2073 656c 662e 736f 7572 6365 5f74   = self.source_t
+0002cdd0: 7970 650a 2020 2020 2020 2020 6966 2073  ype.        if s
+0002cde0: 656c 662e 7374 6172 745f 7469 6d65 2069  elf.start_time i
+0002cdf0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002ce00: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002ce10: 5374 6172 7454 696d 6527 5d20 3d20 7365  StartTime'] = se
+0002ce20: 6c66 2e73 7461 7274 5f74 696d 650a 2020  lf.start_time.  
+0002ce30: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+0002ce40: 6174 7573 2069 7320 6e6f 7420 4e6f 6e65  atus is not None
+0002ce50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002ce60: 7375 6c74 5b27 5374 6174 7573 275d 203d  sult['Status'] =
+0002ce70: 2073 656c 662e 7374 6174 7573 0a20 2020   self.status.   
+0002ce80: 2020 2020 2069 6620 7365 6c66 2e74 656e       if self.ten
+0002ce90: 736f 7262 6f61 7264 5f69 6420 6973 206e  sorboard_id is n
+0002cea0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002ceb0: 2020 2020 2072 6573 756c 745b 2754 656e       result['Ten
+0002cec0: 736f 7262 6f61 7264 4964 275d 203d 2073  sorboardId'] = s
+0002ced0: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
+0002cee0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+0002cef0: 6c66 2e76 6572 626f 7365 2069 7320 6e6f  lf.verbose is no
+0002cf00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002cf10: 2020 2020 7265 7375 6c74 5b27 5665 7262      result['Verb
+0002cf20: 6f73 6527 5d20 3d20 7365 6c66 2e76 6572  ose'] = self.ver
+0002cf30: 626f 7365 0a20 2020 2020 2020 2069 6620  bose.        if 
+0002cf40: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
+0002cf50: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+0002cf60: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002cf70: 745b 2757 6f72 6b73 7061 6365 4964 275d  t['WorkspaceId']
+0002cf80: 203d 2073 656c 662e 776f 726b 7370 6163   = self.workspac
+0002cf90: 655f 6964 0a20 2020 2020 2020 2072 6574  e_id.        ret
+0002cfa0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0002cfb0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0002cfc0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+0002cfd0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+0002cfe0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+0002cff0: 2020 2020 6966 206d 2e67 6574 2827 4469      if m.get('Di
+0002d000: 7370 6c61 794e 616d 6527 2920 6973 206e  splayName') is n
+0002d010: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002d020: 2020 2020 2073 656c 662e 6469 7370 6c61       self.displa
+0002d030: 795f 6e61 6d65 203d 206d 2e67 6574 2827  y_name = m.get('
+0002d040: 4469 7370 6c61 794e 616d 6527 290a 2020  DisplayName').  
+0002d050: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002d060: 456e 6454 696d 6527 2920 6973 206e 6f74  EndTime') is not
+0002d070: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002d080: 2020 2073 656c 662e 656e 645f 7469 6d65     self.end_time
+0002d090: 203d 206d 2e67 6574 2827 456e 6454 696d   = m.get('EndTim
+0002d0a0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+0002d0b0: 2e67 6574 2827 4a6f 6249 6427 2920 6973  .get('JobId') is
+0002d0c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002d0d0: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
+0002d0e0: 6964 203d 206d 2e67 6574 2827 4a6f 6249  id = m.get('JobI
+0002d0f0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
+0002d100: 2e67 6574 2827 4f72 6465 7227 2920 6973  .get('Order') is
+0002d110: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002d120: 2020 2020 2020 2073 656c 662e 6f72 6465         self.orde
+0002d130: 7220 3d20 6d2e 6765 7428 274f 7264 6572  r = m.get('Order
+0002d140: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002d150: 6765 7428 2750 6167 654e 756d 6265 7227  get('PageNumber'
+0002d160: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002d170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002d180: 7061 6765 5f6e 756d 6265 7220 3d20 6d2e  page_number = m.
+0002d190: 6765 7428 2750 6167 654e 756d 6265 7227  get('PageNumber'
+0002d1a0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002d1b0: 6574 2827 5061 6765 5369 7a65 2729 2069  et('PageSize') i
+0002d1c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002d1d0: 2020 2020 2020 2020 7365 6c66 2e70 6167          self.pag
+0002d1e0: 655f 7369 7a65 203d 206d 2e67 6574 2827  e_size = m.get('
+0002d1f0: 5061 6765 5369 7a65 2729 0a20 2020 2020  PageSize').     
+0002d200: 2020 2069 6620 6d2e 6765 7428 2753 6f72     if m.get('Sor
+0002d210: 7442 7927 2920 6973 206e 6f74 204e 6f6e  tBy') is not Non
+0002d220: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002d230: 656c 662e 736f 7274 5f62 7920 3d20 6d2e  elf.sort_by = m.
+0002d240: 6765 7428 2753 6f72 7442 7927 290a 2020  get('SortBy').  
+0002d250: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002d260: 536f 7572 6365 4964 2729 2069 7320 6e6f  SourceId') is no
+0002d270: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002d280: 2020 2020 7365 6c66 2e73 6f75 7263 655f      self.source_
+0002d290: 6964 203d 206d 2e67 6574 2827 536f 7572  id = m.get('Sour
+0002d2a0: 6365 4964 2729 0a20 2020 2020 2020 2069  ceId').        i
+0002d2b0: 6620 6d2e 6765 7428 2753 6f75 7263 6554  f m.get('SourceT
+0002d2c0: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
+0002d2d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002d2e0: 656c 662e 736f 7572 6365 5f74 7970 6520  elf.source_type 
+0002d2f0: 3d20 6d2e 6765 7428 2753 6f75 7263 6554  = m.get('SourceT
+0002d300: 7970 6527 290a 2020 2020 2020 2020 6966  ype').        if
+0002d310: 206d 2e67 6574 2827 5374 6172 7454 696d   m.get('StartTim
+0002d320: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+0002d330: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002d340: 662e 7374 6172 745f 7469 6d65 203d 206d  f.start_time = m
+0002d350: 2e67 6574 2827 5374 6172 7454 696d 6527  .get('StartTime'
+0002d360: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002d370: 6574 2827 5374 6174 7573 2729 2069 7320  et('Status') is 
+0002d380: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002d390: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+0002d3a0: 7320 3d20 6d2e 6765 7428 2753 7461 7475  s = m.get('Statu
+0002d3b0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+0002d3c0: 2e67 6574 2827 5465 6e73 6f72 626f 6172  .get('Tensorboar
+0002d3d0: 6449 6427 2920 6973 206e 6f74 204e 6f6e  dId') is not Non
+0002d3e0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002d3f0: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
+0002d400: 6964 203d 206d 2e67 6574 2827 5465 6e73  id = m.get('Tens
+0002d410: 6f72 626f 6172 6449 6427 290a 2020 2020  orboardId').    
+0002d420: 2020 2020 6966 206d 2e67 6574 2827 5665      if m.get('Ve
+0002d430: 7262 6f73 6527 2920 6973 206e 6f74 204e  rbose') is not N
+0002d440: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002d450: 2073 656c 662e 7665 7262 6f73 6520 3d20   self.verbose = 
+0002d460: 6d2e 6765 7428 2756 6572 626f 7365 2729  m.get('Verbose')
+0002d470: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002d480: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
+0002d490: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002d4a0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+0002d4b0: 6f72 6b73 7061 6365 5f69 6420 3d20 6d2e  orkspace_id = m.
+0002d4c0: 6765 7428 2757 6f72 6b73 7061 6365 4964  get('WorkspaceId
+0002d4d0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+0002d4e0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
+0002d4f0: 6973 7454 656e 736f 7262 6f61 7264 7352  istTensorboardsR
+0002d500: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
+0002d510: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0002d520: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0002d530: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
+0002d540: 6571 7565 7374 5f69 643a 2073 7472 203d  equest_id: str =
+0002d550: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
+0002d560: 656e 736f 7262 6f61 7264 733a 204c 6973  ensorboards: Lis
+0002d570: 745b 5465 6e73 6f72 626f 6172 645d 203d  t[Tensorboard] =
+0002d580: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
+0002d590: 6f74 616c 5f63 6f75 6e74 3a20 696e 7420  otal_count: int 
+0002d5a0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+0002d5b0: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+0002d5c0: 6573 745f 6964 203d 2072 6571 7565 7374  est_id = request
+0002d5d0: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+0002d5e0: 2e74 656e 736f 7262 6f61 7264 7320 3d20  .tensorboards = 
+0002d5f0: 7465 6e73 6f72 626f 6172 6473 0a20 2020  tensorboards.   
+0002d600: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
+0002d610: 636f 756e 7420 3d20 746f 7461 6c5f 636f  count = total_co
+0002d620: 756e 740a 0a20 2020 2064 6566 2076 616c  unt..    def val
+0002d630: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0002d640: 2020 2020 2069 6620 7365 6c66 2e74 656e       if self.ten
+0002d650: 736f 7262 6f61 7264 733a 0a20 2020 2020  sorboards:.     
+0002d660: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+0002d670: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
+0002d680: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0002d690: 2020 2069 6620 6b3a 0a20 2020 2020 2020     if k:.       
+0002d6a0: 2020 2020 2020 2020 2020 2020 206b 2e76               k.v
+0002d6b0: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+0002d6c0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0002d6d0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0002d6e0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+0002d6f0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0002d700: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002d710: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002d720: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0002d730: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0002d740: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0002d750: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
+0002d760: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002d770: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
+0002d780: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
+0002d790: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+0002d7a0: 2072 6573 756c 745b 2754 656e 736f 7262   result['Tensorb
+0002d7b0: 6f61 7264 7327 5d20 3d20 5b5d 0a20 2020  oards'] = [].   
+0002d7c0: 2020 2020 2069 6620 7365 6c66 2e74 656e       if self.ten
+0002d7d0: 736f 7262 6f61 7264 7320 6973 206e 6f74  sorboards is not
+0002d7e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002d7f0: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
+0002d800: 2e74 656e 736f 7262 6f61 7264 733a 0a20  .tensorboards:. 
+0002d810: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0002d820: 6573 756c 745b 2754 656e 736f 7262 6f61  esult['Tensorboa
+0002d830: 7264 7327 5d2e 6170 7065 6e64 286b 2e74  rds'].append(k.t
+0002d840: 6f5f 6d61 7028 2920 6966 206b 2065 6c73  o_map() if k els
+0002d850: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
+0002d860: 6966 2073 656c 662e 746f 7461 6c5f 636f  if self.total_co
+0002d870: 756e 7420 6973 206e 6f74 204e 6f6e 653a  unt is not None:
+0002d880: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002d890: 756c 745b 2754 6f74 616c 436f 756e 7427  ult['TotalCount'
+0002d8a0: 5d20 3d20 7365 6c66 2e74 6f74 616c 5f63  ] = self.total_c
+0002d8b0: 6f75 6e74 0a20 2020 2020 2020 2072 6574  ount.        ret
+0002d8c0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0002d8d0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0002d8e0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+0002d8f0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+0002d900: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+0002d910: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
+0002d920: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
+0002d930: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002d940: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+0002d950: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
+0002d960: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
+0002d970: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
+0002d980: 7320 3d20 5b5d 0a20 2020 2020 2020 2069  s = [].        i
+0002d990: 6620 6d2e 6765 7428 2754 656e 736f 7262  f m.get('Tensorb
+0002d9a0: 6f61 7264 7327 2920 6973 206e 6f74 204e  oards') is not N
+0002d9b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002d9c0: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
+0002d9d0: 2754 656e 736f 7262 6f61 7264 7327 293a  'Tensorboards'):
+0002d9e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002d9f0: 2074 656d 705f 6d6f 6465 6c20 3d20 5465   temp_model = Te
+0002da00: 6e73 6f72 626f 6172 6428 290a 2020 2020  nsorboard().    
+0002da10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002da20: 2e74 656e 736f 7262 6f61 7264 732e 6170  .tensorboards.ap
+0002da30: 7065 6e64 2874 656d 705f 6d6f 6465 6c2e  pend(temp_model.
+0002da40: 6672 6f6d 5f6d 6170 286b 2929 0a20 2020  from_map(k)).   
+0002da50: 2020 2020 2069 6620 6d2e 6765 7428 2754       if m.get('T
+0002da60: 6f74 616c 436f 756e 7427 2920 6973 206e  otalCount') is n
+0002da70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002da80: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
+0002da90: 636f 756e 7420 3d20 6d2e 6765 7428 2754  count = m.get('T
+0002daa0: 6f74 616c 436f 756e 7427 290a 2020 2020  otalCount').    
+0002dab0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0002dac0: 0a0a 636c 6173 7320 4c69 7374 5465 6e73  ..class ListTens
+0002dad0: 6f72 626f 6172 6473 5265 7370 6f6e 7365  orboardsResponse
+0002dae0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+0002daf0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0002db00: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0002db10: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+0002db20: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+0002db30: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+0002db40: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+0002db50: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+0002db60: 793a 204c 6973 7454 656e 736f 7262 6f61  y: ListTensorboa
+0002db70: 7264 7352 6573 706f 6e73 6542 6f64 7920  rdsResponseBody 
+0002db80: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+0002db90: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+0002dba0: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
+0002dbb0: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+0002dbc0: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
+0002dbd0: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
+0002dbe0: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
+0002dbf0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0002dc00: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+0002dc10: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+0002dc20: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
+0002dc30: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
+0002dc40: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0002dc50: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0002dc60: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
+0002dc70: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
+0002dc80: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0002dc90: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0002dca0: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
+0002dcb0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002dcc0: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+0002dcd0: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+0002dce0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+0002dcf0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0002dd00: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0002dd10: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+0002dd20: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0002dd30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002dd40: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0002dd50: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0002dd60: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0002dd70: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+0002dd80: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+0002dd90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002dda0: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+0002ddb0: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+0002ddc0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0002ddd0: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+0002dde0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002ddf0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+0002de00: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+0002de10: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+0002de20: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+0002de30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002de40: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002de50: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+0002de60: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+0002de70: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0002de80: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+0002de90: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+0002dea0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+0002deb0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0002dec0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0002ded0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+0002dee0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002def0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+0002df00: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+0002df10: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+0002df20: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+0002df30: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+0002df40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002df50: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0002df60: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+0002df70: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+0002df80: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+0002df90: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002dfa0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+0002dfb0: 6d6f 6465 6c20 3d20 4c69 7374 5465 6e73  model = ListTens
+0002dfc0: 6f72 626f 6172 6473 5265 7370 6f6e 7365  orboardsResponse
+0002dfd0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
+0002dfe0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+0002dff0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+0002e000: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+0002e010: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0002e020: 660a 0a0a 636c 6173 7320 5374 6172 7454  f...class StartT
+0002e030: 656e 736f 7262 6f61 7264 5265 7175 6573  ensorboardReques
+0002e040: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+0002e050: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+0002e060: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0002e070: 2020 2020 2077 6f72 6b73 7061 6365 5f69       workspace_i
+0002e080: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0002e090: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+0002e0a0: 6c66 2e77 6f72 6b73 7061 6365 5f69 6420  lf.workspace_id 
+0002e0b0: 3d20 776f 726b 7370 6163 655f 6964 0a0a  = workspace_id..
+0002e0c0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0002e0d0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002e0e0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+0002e0f0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0002e100: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0002e110: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+0002e120: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+0002e130: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002e140: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+0002e150: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+0002e160: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0002e170: 2020 6966 2073 656c 662e 776f 726b 7370    if self.worksp
+0002e180: 6163 655f 6964 2069 7320 6e6f 7420 4e6f  ace_id is not No
+0002e190: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002e1a0: 7265 7375 6c74 5b27 576f 726b 7370 6163  result['Workspac
+0002e1b0: 6549 6427 5d20 3d20 7365 6c66 2e77 6f72  eId'] = self.wor
+0002e1c0: 6b73 7061 6365 5f69 640a 2020 2020 2020  kspace_id.      
+0002e1d0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0002e1e0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+0002e1f0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+0002e200: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+0002e210: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+0002e220: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002e230: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
+0002e240: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002e250: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
+0002e260: 6f72 6b73 7061 6365 5f69 6420 3d20 6d2e  orkspace_id = m.
+0002e270: 6765 7428 2757 6f72 6b73 7061 6365 4964  get('WorkspaceId
+0002e280: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+0002e290: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
+0002e2a0: 7461 7274 5465 6e73 6f72 626f 6172 6452  tartTensorboardR
+0002e2b0: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
+0002e2c0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0002e2d0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0002e2e0: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
+0002e2f0: 6571 7565 7374 5f69 643a 2073 7472 203d  equest_id: str =
+0002e300: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
+0002e310: 656e 736f 7262 6f61 7264 5f69 643a 2073  ensorboard_id: s
+0002e320: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+0002e330: 3a0a 2020 2020 2020 2020 7365 6c66 2e72  :.        self.r
+0002e340: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
+0002e350: 6573 745f 6964 0a20 2020 2020 2020 2073  est_id.        s
+0002e360: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
+0002e370: 6964 203d 2074 656e 736f 7262 6f61 7264  id = tensorboard
+0002e380: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
+0002e390: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0002e3a0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+0002e3b0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0002e3c0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0002e3d0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+0002e3e0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0002e3f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002e400: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002e410: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0002e420: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0002e430: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0002e440: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
+0002e450: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002e460: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
+0002e470: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
+0002e480: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+0002e490: 2069 6620 7365 6c66 2e74 656e 736f 7262   if self.tensorb
+0002e4a0: 6f61 7264 5f69 6420 6973 206e 6f74 204e  oard_id is not N
+0002e4b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002e4c0: 2072 6573 756c 745b 2754 656e 736f 7262   result['Tensorb
+0002e4d0: 6f61 7264 4964 275d 203d 2073 656c 662e  oardId'] = self.
+0002e4e0: 7465 6e73 6f72 626f 6172 645f 6964 0a20  tensorboard_id. 
+0002e4f0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0002e500: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0002e510: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+0002e520: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+0002e530: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+0002e540: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0002e550: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+0002e560: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002e570: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002e580: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
+0002e590: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+0002e5a0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002e5b0: 6574 2827 5465 6e73 6f72 626f 6172 6449  et('TensorboardI
+0002e5c0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002e5d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002e5e0: 662e 7465 6e73 6f72 626f 6172 645f 6964  f.tensorboard_id
+0002e5f0: 203d 206d 2e67 6574 2827 5465 6e73 6f72   = m.get('Tensor
+0002e600: 626f 6172 6449 6427 290a 2020 2020 2020  boardId').      
+0002e610: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+0002e620: 636c 6173 7320 5374 6172 7454 656e 736f  class StartTenso
+0002e630: 7262 6f61 7264 5265 7370 6f6e 7365 2854  rboardResponse(T
+0002e640: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0002e650: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0002e660: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0002e670: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
+0002e680: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
+0002e690: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+0002e6a0: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
+0002e6b0: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+0002e6c0: 2053 7461 7274 5465 6e73 6f72 626f 6172   StartTensorboar
+0002e6d0: 6452 6573 706f 6e73 6542 6f64 7920 3d20  dResponseBody = 
+0002e6e0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+0002e6f0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+0002e700: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
+0002e710: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+0002e720: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+0002e730: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
+0002e740: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
+0002e750: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+0002e760: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+0002e770: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+0002e780: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
+0002e790: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
+0002e7a0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+0002e7b0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+0002e7c0: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
+0002e7d0: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
+0002e7e0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+0002e7f0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+0002e800: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
+0002e810: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+0002e820: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
+0002e830: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
+0002e840: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+0002e850: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0002e860: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0002e870: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+0002e880: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0002e890: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002e8a0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0002e8b0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0002e8c0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0002e8d0: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
+0002e8e0: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
+0002e8f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002e900: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
+0002e910: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
+0002e920: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+0002e930: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
+0002e940: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002e950: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
+0002e960: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
+0002e970: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+0002e980: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
+0002e990: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002e9a0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002e9b0: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
+0002e9c0: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
+0002e9d0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0002e9e0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+0002e9f0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+0002ea00: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+0002ea10: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+0002ea20: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+0002ea30: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
+0002ea40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002ea50: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+0002ea60: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
+0002ea70: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+0002ea80: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
+0002ea90: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
+0002eaa0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002eab0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0002eac0: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
+0002ead0: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
+0002eae0: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
+0002eaf0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002eb00: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+0002eb10: 6465 6c20 3d20 5374 6172 7454 656e 736f  del = StartTenso
+0002eb20: 7262 6f61 7264 5265 7370 6f6e 7365 426f  rboardResponseBo
+0002eb30: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+0002eb40: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+0002eb50: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+0002eb60: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+0002eb70: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0002eb80: 0a0a 636c 6173 7320 5374 6f70 4a6f 6252  ..class StopJobR
+0002eb90: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
+0002eba0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0002ebb0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0002ebc0: 2073 656c 662c 0a20 2020 2020 2020 206a   self,.        j
+0002ebd0: 6f62 5f69 643a 2073 7472 203d 204e 6f6e  ob_id: str = Non
+0002ebe0: 652c 0a20 2020 2020 2020 2072 6571 7565  e,.        reque
+0002ebf0: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+0002ec00: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+0002ec10: 2020 7365 6c66 2e6a 6f62 5f69 6420 3d20    self.job_id = 
+0002ec20: 6a6f 625f 6964 0a20 2020 2020 2020 2073  job_id.        s
+0002ec30: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+0002ec40: 2072 6571 7565 7374 5f69 640a 0a20 2020   request_id..   
+0002ec50: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+0002ec60: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+0002ec70: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+0002ec80: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0002ec90: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+0002eca0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0002ecb0: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0002ecc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002ecd0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0002ece0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0002ecf0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0002ed00: 6620 7365 6c66 2e6a 6f62 5f69 6420 6973  f self.job_id is
+0002ed10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002ed20: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
+0002ed30: 6f62 4964 275d 203d 2073 656c 662e 6a6f  obId'] = self.jo
+0002ed40: 625f 6964 0a20 2020 2020 2020 2069 6620  b_id.        if 
+0002ed50: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0002ed60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002ed70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002ed80: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+0002ed90: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+0002eda0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0002edb0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0002edc0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+0002edd0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+0002ede0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+0002edf0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0002ee00: 206d 2e67 6574 2827 4a6f 6249 6427 2920   m.get('JobId') 
+0002ee10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002ee20: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
+0002ee30: 625f 6964 203d 206d 2e67 6574 2827 4a6f  b_id = m.get('Jo
+0002ee40: 6249 6427 290a 2020 2020 2020 2020 6966  bId').        if
+0002ee50: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+0002ee60: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002ee70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002ee80: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
+0002ee90: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+0002eea0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0002eeb0: 2073 656c 660a 0a0a 636c 6173 7320 5374   self...class St
+0002eec0: 6f70 4a6f 6252 6573 706f 6e73 6528 5465  opJobResponse(Te
+0002eed0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0002eee0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+0002eef0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0002ef00: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
+0002ef10: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
+0002ef20: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
+0002ef30: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
+0002ef40: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
+0002ef50: 5374 6f70 4a6f 6252 6573 706f 6e73 6542  StopJobResponseB
+0002ef60: 6f64 7920 3d20 4e6f 6e65 2c0a 2020 2020  ody = None,.    
+0002ef70: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0002ef80: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+0002ef90: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
+0002efa0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+0002efb0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+0002efc0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
+0002efd0: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
+0002efe0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+0002eff0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+0002f000: 5f72 6571 7569 7265 6428 7365 6c66 2e68  _required(self.h
+0002f010: 6561 6465 7273 2c20 2768 6561 6465 7273  eaders, 'headers
+0002f020: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0002f030: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+0002f040: 6428 7365 6c66 2e73 7461 7475 735f 636f  d(self.status_co
+0002f050: 6465 2c20 2773 7461 7475 735f 636f 6465  de, 'status_code
+0002f060: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
+0002f070: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+0002f080: 6428 7365 6c66 2e62 6f64 792c 2027 626f  d(self.body, 'bo
+0002f090: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
+0002f0a0: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
+0002f0b0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0002f0c0: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
+0002f0d0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0002f0e0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0002f0f0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+0002f100: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+0002f110: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+0002f120: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0002f130: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+0002f140: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+0002f150: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002f160: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
+0002f170: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002f180: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
+0002f190: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
+0002f1a0: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
+0002f1b0: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
+0002f1c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002f1d0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002f1e0: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
+0002f1f0: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
+0002f200: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002f210: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
+0002f220: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002f230: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
+0002f240: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
+0002f250: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0002f260: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+0002f270: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+0002f280: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+0002f290: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+0002f2a0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+0002f2b0: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+0002f2c0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+0002f2d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002f2e0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+0002f2f0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+0002f300: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002f310: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+0002f320: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002f330: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+0002f340: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+0002f350: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+0002f360: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+0002f370: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+0002f380: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+0002f390: 656d 705f 6d6f 6465 6c20 3d20 5374 6f70  emp_model = Stop
+0002f3a0: 4a6f 6252 6573 706f 6e73 6542 6f64 7928  JobResponseBody(
+0002f3b0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0002f3c0: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
+0002f3d0: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
+0002f3e0: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
+0002f3f0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+0002f400: 6c61 7373 2053 746f 7054 656e 736f 7262  lass StopTensorb
+0002f410: 6f61 7264 5265 7175 6573 7428 5465 614d  oardRequest(TeaM
+0002f420: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0002f430: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0002f440: 2073 656c 662c 0a20 2020 2020 2020 2077   self,.        w
+0002f450: 6f72 6b73 7061 6365 5f69 643a 2073 7472  orkspace_id: str
+0002f460: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+0002f470: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+0002f480: 6b73 7061 6365 5f69 6420 3d20 776f 726b  kspace_id = work
+0002f490: 7370 6163 655f 6964 0a0a 2020 2020 6465  space_id..    de
+0002f4a0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+0002f4b0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0002f4c0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+0002f4d0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+0002f4e0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+0002f4f0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+0002f500: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+0002f510: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002f520: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+0002f530: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+0002f540: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+0002f550: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+0002f560: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002f570: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002f580: 5b27 576f 726b 7370 6163 6549 6427 5d20  ['WorkspaceId'] 
+0002f590: 3d20 7365 6c66 2e77 6f72 6b73 7061 6365  = self.workspace
+0002f5a0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+0002f5b0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0002f5c0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0002f5d0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+0002f5e0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0002f5f0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0002f600: 2020 2069 6620 6d2e 6765 7428 2757 6f72     if m.get('Wor
+0002f610: 6b73 7061 6365 4964 2729 2069 7320 6e6f  kspaceId') is no
+0002f620: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002f630: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
+0002f640: 6365 5f69 6420 3d20 6d2e 6765 7428 2757  ce_id = m.get('W
+0002f650: 6f72 6b73 7061 6365 4964 2729 0a20 2020  orkspaceId').   
+0002f660: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0002f670: 0a0a 0a63 6c61 7373 2053 746f 7054 656e  ...class StopTen
+0002f680: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
+0002f690: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
+0002f6a0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0002f6b0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0002f6c0: 2020 2020 2020 2020 7265 7175 6573 745f          request_
+0002f6d0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0002f6e0: 2020 2020 2020 2020 7465 6e73 6f72 626f          tensorbo
+0002f6f0: 6172 645f 6964 3a20 7374 7220 3d20 4e6f  ard_id: str = No
+0002f700: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0002f710: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+0002f720: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
+0002f730: 2020 2020 2020 2020 7365 6c66 2e74 656e          self.ten
+0002f740: 736f 7262 6f61 7264 5f69 6420 3d20 7465  sorboard_id = te
+0002f750: 6e73 6f72 626f 6172 645f 6964 0a0a 2020  nsorboard_id..  
+0002f760: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+0002f770: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+0002f780: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+0002f790: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+0002f7a0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+0002f7b0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0002f7c0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0002f7d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002f7e0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0002f7f0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0002f800: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0002f810: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+0002f820: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0002f830: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002f840: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
+0002f850: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
+0002f860: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+0002f870: 662e 7465 6e73 6f72 626f 6172 645f 6964  f.tensorboard_id
+0002f880: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002f890: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002f8a0: 5b27 5465 6e73 6f72 626f 6172 6449 6427  ['TensorboardId'
+0002f8b0: 5d20 3d20 7365 6c66 2e74 656e 736f 7262  ] = self.tensorb
+0002f8c0: 6f61 7264 5f69 640a 2020 2020 2020 2020  oard_id.        
+0002f8d0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0002f8e0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+0002f8f0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+0002f900: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0002f910: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0002f920: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002f930: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
+0002f940: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002f950: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+0002f960: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
+0002f970: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
+0002f980: 2020 2069 6620 6d2e 6765 7428 2754 656e     if m.get('Ten
+0002f990: 736f 7262 6f61 7264 4964 2729 2069 7320  sorboardId') is 
+0002f9a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002f9b0: 2020 2020 2020 7365 6c66 2e74 656e 736f        self.tenso
+0002f9c0: 7262 6f61 7264 5f69 6420 3d20 6d2e 6765  rboard_id = m.ge
+0002f9d0: 7428 2754 656e 736f 7262 6f61 7264 4964  t('TensorboardId
+0002f9e0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+0002f9f0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
+0002fa00: 746f 7054 656e 736f 7262 6f61 7264 5265  topTensorboardRe
+0002fa10: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+0002fa20: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0002fa30: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+0002fa40: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+0002fa50: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+0002fa60: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0002fa70: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
+0002fa80: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+0002fa90: 2020 2062 6f64 793a 2053 746f 7054 656e     body: StopTen
+0002faa0: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
+0002fab0: 426f 6479 203d 204e 6f6e 652c 0a20 2020  Body = None,.   
+0002fac0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+0002fad0: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
+0002fae0: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
+0002faf0: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+0002fb00: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
+0002fb10: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
+0002fb20: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
+0002fb30: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+0002fb40: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+0002fb50: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+0002fb60: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
+0002fb70: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
+0002fb80: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+0002fb90: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
+0002fba0: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
+0002fbb0: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
+0002fbc0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+0002fbd0: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
+0002fbe0: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
+0002fbf0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+0002fc00: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+0002fc10: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+0002fc20: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0002fc30: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0002fc40: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
+0002fc50: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+0002fc60: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+0002fc70: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0002fc80: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+0002fc90: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+0002fca0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0002fcb0: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
+0002fcc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002fcd0: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
+0002fce0: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
+0002fcf0: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
+0002fd00: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0002fd10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002fd20: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002fd30: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
+0002fd40: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0002fd50: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002fd60: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
+0002fd70: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002fd80: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
+0002fd90: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
+0002fda0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+0002fdb0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
+0002fdc0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
+0002fdd0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
+0002fde0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0002fdf0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0002fe00: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+0002fe10: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+0002fe20: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002fe30: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+0002fe40: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+0002fe50: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002fe60: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+0002fe70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002fe80: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0002fe90: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+0002fea0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+0002feb0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002fec0: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+0002fed0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002fee0: 7465 6d70 5f6d 6f64 656c 203d 2053 746f  temp_model = Sto
+0002fef0: 7054 656e 736f 7262 6f61 7264 5265 7370  pTensorboardResp
+0002ff00: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+0002ff10: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0002ff20: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+0002ff30: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+0002ff40: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0002ff50: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
+0002ff60: 6461 7465 4a6f 6252 6571 7565 7374 2854  dateJobRequest(T
+0002ff70: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0002ff80: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0002ff90: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0002ffa0: 2020 7072 696f 7269 7479 3a20 696e 7420    priority: int 
+0002ffb0: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+0002ffc0: 2020 2020 2020 2073 656c 662e 7072 696f         self.prio
+0002ffd0: 7269 7479 203d 2070 7269 6f72 6974 790a  rity = priority.
+0002ffe0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0002fff0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00030000: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+00030010: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00030020: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00030030: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00030040: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00030050: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00030060: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00030070: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00030080: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00030090: 2020 2069 6620 7365 6c66 2e70 7269 6f72     if self.prior
+000300a0: 6974 7920 6973 206e 6f74 204e 6f6e 653a  ity is not None:
+000300b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000300c0: 756c 745b 2750 7269 6f72 6974 7927 5d20  ult['Priority'] 
+000300d0: 3d20 7365 6c66 2e70 7269 6f72 6974 790a  = self.priority.
+000300e0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000300f0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00030100: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00030110: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00030120: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00030130: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00030140: 6620 6d2e 6765 7428 2750 7269 6f72 6974  f m.get('Priorit
+00030150: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+00030160: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00030170: 662e 7072 696f 7269 7479 203d 206d 2e67  f.priority = m.g
+00030180: 6574 2827 5072 696f 7269 7479 2729 0a20  et('Priority'). 
+00030190: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000301a0: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
+000301b0: 654a 6f62 5265 7370 6f6e 7365 426f 6479  eJobResponseBody
+000301c0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+000301d0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+000301e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000301f0: 2020 2020 6a6f 625f 6964 3a20 7374 7220      job_id: str 
+00030200: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00030210: 7265 7175 6573 745f 6964 3a20 7374 7220  request_id: str 
+00030220: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+00030230: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
+00030240: 6964 203d 206a 6f62 5f69 640a 2020 2020  id = job_id.    
+00030250: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+00030260: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
+00030270: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00030280: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00030290: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+000302a0: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+000302b0: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+000302c0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+000302d0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+000302e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000302f0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00030300: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00030310: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00030320: 2020 2020 6966 2073 656c 662e 6a6f 625f      if self.job_
+00030330: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00030340: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00030350: 6c74 5b27 4a6f 6249 6427 5d20 3d20 7365  lt['JobId'] = se
+00030360: 6c66 2e6a 6f62 5f69 640a 2020 2020 2020  lf.job_id.      
+00030370: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
+00030380: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
+00030390: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000303a0: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
+000303b0: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
+000303c0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+000303d0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+000303e0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+000303f0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+00030400: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+00030410: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+00030420: 2020 2069 6620 6d2e 6765 7428 274a 6f62     if m.get('Job
+00030430: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+00030440: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00030450: 6c66 2e6a 6f62 5f69 6420 3d20 6d2e 6765  lf.job_id = m.ge
+00030460: 7428 274a 6f62 4964 2729 0a20 2020 2020  t('JobId').     
+00030470: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
+00030480: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
+00030490: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000304a0: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+000304b0: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
+000304c0: 7374 4964 2729 0a20 2020 2020 2020 2072  stId').        r
+000304d0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+000304e0: 7373 2055 7064 6174 654a 6f62 5265 7370  ss UpdateJobResp
+000304f0: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+00030500: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00030510: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00030520: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
+00030530: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
+00030540: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00030550: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
+00030560: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00030570: 2062 6f64 793a 2055 7064 6174 654a 6f62   body: UpdateJob
+00030580: 5265 7370 6f6e 7365 426f 6479 203d 204e  ResponseBody = N
+00030590: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+000305a0: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+000305b0: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
+000305c0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+000305d0: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
+000305e0: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
+000305f0: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
+00030600: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00030610: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00030620: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+00030630: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
+00030640: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
+00030650: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+00030660: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+00030670: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
+00030680: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
+00030690: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+000306a0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+000306b0: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
+000306c0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+000306d0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
+000306e0: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
+000306f0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
+00030700: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00030710: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00030720: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+00030730: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00030740: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00030750: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00030760: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00030770: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00030780: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+00030790: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+000307a0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000307b0: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+000307c0: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+000307d0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+000307e0: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+000307f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00030800: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+00030810: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+00030820: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+00030830: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+00030840: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00030850: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+00030860: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+00030870: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+00030880: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00030890: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+000308a0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+000308b0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+000308c0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+000308d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000308e0: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
+000308f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00030900: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+00030910: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
+00030920: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
+00030930: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
+00030940: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
+00030950: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00030960: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+00030970: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
+00030980: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
+00030990: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
+000309a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000309b0: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
+000309c0: 656c 203d 2055 7064 6174 654a 6f62 5265  el = UpdateJobRe
+000309d0: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
+000309e0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
+000309f0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
+00030a00: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
+00030a10: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
+00030a20: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00030a30: 5570 6461 7465 5465 6e73 6f72 626f 6172  UpdateTensorboar
+00030a40: 6452 6571 7565 7374 2854 6561 4d6f 6465  dRequest(TeaMode
+00030a50: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00030a60: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00030a70: 6c66 2c0a 2020 2020 2020 2020 6d61 785f  lf,.        max_
+00030a80: 7275 6e6e 696e 675f 7469 6d65 5f6d 696e  running_time_min
+00030a90: 7574 6573 3a20 696e 7420 3d20 4e6f 6e65  utes: int = None
+00030aa0: 2c0a 2020 2020 2020 2020 776f 726b 7370  ,.        worksp
+00030ab0: 6163 655f 6964 3a20 7374 7220 3d20 4e6f  ace_id: str = No
+00030ac0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+00030ad0: 2020 2073 656c 662e 6d61 785f 7275 6e6e     self.max_runn
+00030ae0: 696e 675f 7469 6d65 5f6d 696e 7574 6573  ing_time_minutes
+00030af0: 203d 206d 6178 5f72 756e 6e69 6e67 5f74   = max_running_t
+00030b00: 696d 655f 6d69 6e75 7465 730a 2020 2020  ime_minutes.    
+00030b10: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
+00030b20: 6365 5f69 6420 3d20 776f 726b 7370 6163  ce_id = workspac
+00030b30: 655f 6964 0a0a 2020 2020 6465 6620 7661  e_id..    def va
+00030b40: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00030b50: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00030b60: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00030b70: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00030b80: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00030b90: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00030ba0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00030bb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00030bc0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00030bd0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00030be0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00030bf0: 6d61 785f 7275 6e6e 696e 675f 7469 6d65  max_running_time
+00030c00: 5f6d 696e 7574 6573 2069 7320 6e6f 7420  _minutes is not 
+00030c10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00030c20: 2020 7265 7375 6c74 5b27 4d61 7852 756e    result['MaxRun
+00030c30: 6e69 6e67 5469 6d65 4d69 6e75 7465 7327  ningTimeMinutes'
+00030c40: 5d20 3d20 7365 6c66 2e6d 6178 5f72 756e  ] = self.max_run
+00030c50: 6e69 6e67 5f74 696d 655f 6d69 6e75 7465  ning_time_minute
+00030c60: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+00030c70: 662e 776f 726b 7370 6163 655f 6964 2069  f.workspace_id i
+00030c80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00030c90: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00030ca0: 576f 726b 7370 6163 6549 6427 5d20 3d20  WorkspaceId'] = 
+00030cb0: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
+00030cc0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+00030cd0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00030ce0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+00030cf0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
+00030d00: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00030d10: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00030d20: 2069 6620 6d2e 6765 7428 274d 6178 5275   if m.get('MaxRu
+00030d30: 6e6e 696e 6754 696d 654d 696e 7574 6573  nningTimeMinutes
+00030d40: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00030d50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00030d60: 2e6d 6178 5f72 756e 6e69 6e67 5f74 696d  .max_running_tim
+00030d70: 655f 6d69 6e75 7465 7320 3d20 6d2e 6765  e_minutes = m.ge
+00030d80: 7428 274d 6178 5275 6e6e 696e 6754 696d  t('MaxRunningTim
+00030d90: 654d 696e 7574 6573 2729 0a20 2020 2020  eMinutes').     
+00030da0: 2020 2069 6620 6d2e 6765 7428 2757 6f72     if m.get('Wor
+00030db0: 6b73 7061 6365 4964 2729 2069 7320 6e6f  kspaceId') is no
+00030dc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00030dd0: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
+00030de0: 6365 5f69 6420 3d20 6d2e 6765 7428 2757  ce_id = m.get('W
+00030df0: 6f72 6b73 7061 6365 4964 2729 0a20 2020  orkspaceId').   
+00030e00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00030e10: 0a0a 0a63 6c61 7373 2055 7064 6174 6554  ...class UpdateT
+00030e20: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
+00030e30: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
+00030e40: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00030e50: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00030e60: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
+00030e70: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
+00030e80: 2c0a 2020 2020 2020 2020 7465 6e73 6f72  ,.        tensor
+00030e90: 626f 6172 645f 6964 3a20 7374 7220 3d20  board_id: str = 
+00030ea0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00030eb0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+00030ec0: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
+00030ed0: 640a 2020 2020 2020 2020 7365 6c66 2e74  d.        self.t
+00030ee0: 656e 736f 7262 6f61 7264 5f69 6420 3d20  ensorboard_id = 
+00030ef0: 7465 6e73 6f72 626f 6172 645f 6964 0a0a  tensorboard_id..
+00030f00: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00030f10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00030f20: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+00030f30: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00030f40: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00030f50: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
+00030f60: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+00030f70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00030f80: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00030f90: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00030fa0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00030fb0: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
+00030fc0: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
+00030fd0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00030fe0: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
+00030ff0: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
+00031000: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00031010: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
+00031020: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00031030: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00031040: 6c74 5b27 5465 6e73 6f72 626f 6172 6449  lt['TensorboardI
+00031050: 6427 5d20 3d20 7365 6c66 2e74 656e 736f  d'] = self.tenso
+00031060: 7262 6f61 7264 5f69 640a 2020 2020 2020  rboard_id.      
+00031070: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00031080: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00031090: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+000310a0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+000310b0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+000310c0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000310d0: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
+000310e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000310f0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+00031100: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
+00031110: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
+00031120: 2020 2020 2069 6620 6d2e 6765 7428 2754       if m.get('T
+00031130: 656e 736f 7262 6f61 7264 4964 2729 2069  ensorboardId') i
+00031140: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00031150: 2020 2020 2020 2020 7365 6c66 2e74 656e          self.ten
+00031160: 736f 7262 6f61 7264 5f69 6420 3d20 6d2e  sorboard_id = m.
+00031170: 6765 7428 2754 656e 736f 7262 6f61 7264  get('Tensorboard
+00031180: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
+00031190: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+000311a0: 2055 7064 6174 6554 656e 736f 7262 6f61   UpdateTensorboa
+000311b0: 7264 5265 7370 6f6e 7365 2854 6561 4d6f  rdResponse(TeaMo
+000311c0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+000311d0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000311e0: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+000311f0: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+00031200: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+00031210: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+00031220: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+00031230: 2020 2020 2020 2062 6f64 793a 2055 7064         body: Upd
+00031240: 6174 6554 656e 736f 7262 6f61 7264 5265  ateTensorboardRe
+00031250: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
+00031260: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+00031270: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+00031280: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
+00031290: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+000312a0: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
+000312b0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+000312c0: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
+000312d0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+000312e0: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
+000312f0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
+00031300: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
+00031310: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+00031320: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00031330: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
+00031340: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
+00031350: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
+00031360: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
+00031370: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
+00031380: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
+00031390: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+000313a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000313b0: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
+000313c0: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
+000313d0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+000313e0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+000313f0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00031400: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00031410: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00031420: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+00031430: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00031440: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+00031450: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
+00031460: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00031470: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00031480: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
+00031490: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
+000314a0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+000314b0: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+000314c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000314d0: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
+000314e0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
+000314f0: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
+00031500: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
+00031510: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00031520: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
+00031530: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
+00031540: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00031550: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00031560: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+00031570: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
+00031580: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
+00031590: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+000315a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000315b0: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+000315c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000315d0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+000315e0: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+000315f0: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+00031600: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00031610: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00031620: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00031630: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00031640: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+00031650: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+00031660: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+00031670: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00031680: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00031690: 203d 2055 7064 6174 6554 656e 736f 7262   = UpdateTensorb
+000316a0: 6f61 7264 5265 7370 6f6e 7365 426f 6479  oardResponseBody
+000316b0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+000316c0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
+000316d0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
+000316e0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
+000316f0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.8/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO` & `alibabacloud_pai-dlc20201203-1.2.9/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pai-dlc20201203
-Version: 1.2.8
+Version: 1.2.9
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.8/setup.py` & `alibabacloud_pai-dlc20201203-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pai-dlc20201203.
 
-Created on 21/07/2023
+Created on 26/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pai_dlc20201203"
 NAME = "alibabacloud_pai-dlc20201203" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud pai-dlc (20201203) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.10, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

