# Comparing `tmp/antchain_blockchain-1.26.33.tar.gz` & `tmp/antchain_blockchain-1.26.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_blockchain-1.26.33.tar", last modified: Thu Feb  9 08:51:17 2023, max compression
+gzip compressed data, was "dist/antchain_blockchain-1.26.36.tar", last modified: Wed Jul 26 02:54:34 2023, max compression
```

## Comparing `antchain_blockchain-1.26.33.tar` & `antchain_blockchain-1.26.36.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 08:51:17.000000 antchain_blockchain-1.26.33/
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-09 08:51:16.000000 antchain_blockchain-1.26.33/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-09 08:51:16.000000 antchain_blockchain-1.26.33/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2206 2023-02-09 08:51:17.000000 antchain_blockchain-1.26.33/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      825 2023-02-09 08:51:16.000000 antchain_blockchain-1.26.33/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1011 2023-02-09 08:51:16.000000 antchain_blockchain-1.26.33/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 08:51:17.000000 antchain_blockchain-1.26.33/antchain_blockchain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2206 2023-02-09 08:51:17.000000 antchain_blockchain-1.26.33/antchain_blockchain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      379 2023-02-09 08:51:17.000000 antchain_blockchain-1.26.33/antchain_blockchain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-09 08:51:17.000000 antchain_blockchain-1.26.33/antchain_blockchain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-02-09 08:51:17.000000 antchain_blockchain-1.26.33/antchain_blockchain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-02-09 08:51:17.000000 antchain_blockchain-1.26.33/antchain_blockchain.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-09 08:51:17.000000 antchain_blockchain-1.26.33/antchain_sdk_blockchain/
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-09 08:51:16.000000 antchain_blockchain-1.26.33/antchain_sdk_blockchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1399403 2023-02-09 08:51:16.000000 antchain_blockchain-1.26.33/antchain_sdk_blockchain/client.py
--rw-r--r--   0 root         (0) root         (0)  2818487 2023-02-09 08:51:16.000000 antchain_blockchain-1.26.33/antchain_sdk_blockchain/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-09 08:51:17.000000 antchain_blockchain-1.26.33/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2523 2023-02-09 08:51:16.000000 antchain_blockchain-1.26.33/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2206 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      825 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/antchain_blockchain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2206 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/antchain_blockchain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/antchain_blockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/antchain_blockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/antchain_blockchain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/antchain_blockchain.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/antchain_sdk_blockchain/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/antchain_sdk_blockchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1433889 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/antchain_sdk_blockchain/client.py
+-rw-r--r--   0 root         (0) root         (0)  2898767 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/antchain_sdk_blockchain/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-07-26 02:54:34.000000 antchain_blockchain-1.26.36/setup.py
```

### Comparing `antchain_blockchain-1.26.33/LICENSE` & `antchain_blockchain-1.26.36/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_blockchain-1.26.33/PKG-INFO` & `antchain_blockchain-1.26.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_blockchain
-Version: 1.26.33
+Version: 1.26.36
 Summary: Ant Chain BLOCKCHAIN SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_blockchain-1.26.33/README-CN.md` & `antchain_blockchain-1.26.36/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_blockchain-1.26.33/README.md` & `antchain_blockchain-1.26.36/README.md`

 * *Files identical despite different names*

### Comparing `antchain_blockchain-1.26.33/antchain_blockchain.egg-info/PKG-INFO` & `antchain_blockchain-1.26.36/antchain_blockchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-blockchain
-Version: 1.26.33
+Version: 1.26.36
 Summary: Ant Chain BLOCKCHAIN SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_blockchain-1.26.33/antchain_sdk_blockchain/client.py` & `antchain_blockchain-1.26.36/antchain_sdk_blockchain/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.26.33',
+                    'sdk_version': '1.26.36',
                     '_prod_code': 'BLOCKCHAIN',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -198,15 +198,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.26.33',
+                    'sdk_version': '1.26.36',
                     '_prod_code': 'BLOCKCHAIN',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -13691,14 +13691,798 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             blockchain_models.QueryApiDwhbTransactionResponse(),
             await self.do_request_async('1.0', 'baas.api.dwhb.transaction.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def create_caas_application_manage(
+        self,
+        request: blockchain_models.CreateCaasApplicationManageRequest,
+    ) -> blockchain_models.CreateCaasApplicationManageResponse:
+        """
+        Description: 新建应用
+        Summary: 新建应用
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_caas_application_manage_ex(request, headers, runtime)
+
+    async def create_caas_application_manage_async(
+        self,
+        request: blockchain_models.CreateCaasApplicationManageRequest,
+    ) -> blockchain_models.CreateCaasApplicationManageResponse:
+        """
+        Description: 新建应用
+        Summary: 新建应用
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_caas_application_manage_ex_async(request, headers, runtime)
+
+    def create_caas_application_manage_ex(
+        self,
+        request: blockchain_models.CreateCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.CreateCaasApplicationManageResponse:
+        """
+        Description: 新建应用
+        Summary: 新建应用
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.CreateCaasApplicationManageResponse(),
+            self.do_request('1.0', 'baas.caas.application.manage.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_caas_application_manage_ex_async(
+        self,
+        request: blockchain_models.CreateCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.CreateCaasApplicationManageResponse:
+        """
+        Description: 新建应用
+        Summary: 新建应用
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.CreateCaasApplicationManageResponse(),
+            await self.do_request_async('1.0', 'baas.caas.application.manage.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_caas_application_manage(
+        self,
+        request: blockchain_models.PagequeryCaasApplicationManageRequest,
+    ) -> blockchain_models.PagequeryCaasApplicationManageResponse:
+        """
+        Description: 应用列表查询
+        Summary: 应用列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_caas_application_manage_ex(request, headers, runtime)
+
+    async def pagequery_caas_application_manage_async(
+        self,
+        request: blockchain_models.PagequeryCaasApplicationManageRequest,
+    ) -> blockchain_models.PagequeryCaasApplicationManageResponse:
+        """
+        Description: 应用列表查询
+        Summary: 应用列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_caas_application_manage_ex_async(request, headers, runtime)
+
+    def pagequery_caas_application_manage_ex(
+        self,
+        request: blockchain_models.PagequeryCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.PagequeryCaasApplicationManageResponse:
+        """
+        Description: 应用列表查询
+        Summary: 应用列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.PagequeryCaasApplicationManageResponse(),
+            self.do_request('1.0', 'baas.caas.application.manage.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_caas_application_manage_ex_async(
+        self,
+        request: blockchain_models.PagequeryCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.PagequeryCaasApplicationManageResponse:
+        """
+        Description: 应用列表查询
+        Summary: 应用列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.PagequeryCaasApplicationManageResponse(),
+            await self.do_request_async('1.0', 'baas.caas.application.manage.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_caas_application_manage(
+        self,
+        request: blockchain_models.GetCaasApplicationManageRequest,
+    ) -> blockchain_models.GetCaasApplicationManageResponse:
+        """
+        Description: 查看sk
+        Summary: 查看sk
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_caas_application_manage_ex(request, headers, runtime)
+
+    async def get_caas_application_manage_async(
+        self,
+        request: blockchain_models.GetCaasApplicationManageRequest,
+    ) -> blockchain_models.GetCaasApplicationManageResponse:
+        """
+        Description: 查看sk
+        Summary: 查看sk
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_caas_application_manage_ex_async(request, headers, runtime)
+
+    def get_caas_application_manage_ex(
+        self,
+        request: blockchain_models.GetCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.GetCaasApplicationManageResponse:
+        """
+        Description: 查看sk
+        Summary: 查看sk
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.GetCaasApplicationManageResponse(),
+            self.do_request('1.0', 'baas.caas.application.manage.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_caas_application_manage_ex_async(
+        self,
+        request: blockchain_models.GetCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.GetCaasApplicationManageResponse:
+        """
+        Description: 查看sk
+        Summary: 查看sk
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.GetCaasApplicationManageResponse(),
+            await self.do_request_async('1.0', 'baas.caas.application.manage.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_caas_application_manage(
+        self,
+        request: blockchain_models.QueryCaasApplicationManageRequest,
+    ) -> blockchain_models.QueryCaasApplicationManageResponse:
+        """
+        Description: 查询合约绑定关系
+        Summary: 查询合约绑定关系
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_caas_application_manage_ex(request, headers, runtime)
+
+    async def query_caas_application_manage_async(
+        self,
+        request: blockchain_models.QueryCaasApplicationManageRequest,
+    ) -> blockchain_models.QueryCaasApplicationManageResponse:
+        """
+        Description: 查询合约绑定关系
+        Summary: 查询合约绑定关系
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_caas_application_manage_ex_async(request, headers, runtime)
+
+    def query_caas_application_manage_ex(
+        self,
+        request: blockchain_models.QueryCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.QueryCaasApplicationManageResponse:
+        """
+        Description: 查询合约绑定关系
+        Summary: 查询合约绑定关系
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.QueryCaasApplicationManageResponse(),
+            self.do_request('1.0', 'baas.caas.application.manage.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_caas_application_manage_ex_async(
+        self,
+        request: blockchain_models.QueryCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.QueryCaasApplicationManageResponse:
+        """
+        Description: 查询合约绑定关系
+        Summary: 查询合约绑定关系
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.QueryCaasApplicationManageResponse(),
+            await self.do_request_async('1.0', 'baas.caas.application.manage.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def unbind_caas_application_manage(
+        self,
+        request: blockchain_models.UnbindCaasApplicationManageRequest,
+    ) -> blockchain_models.UnbindCaasApplicationManageResponse:
+        """
+        Description: 解除授权
+        Summary: 解除授权
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.unbind_caas_application_manage_ex(request, headers, runtime)
+
+    async def unbind_caas_application_manage_async(
+        self,
+        request: blockchain_models.UnbindCaasApplicationManageRequest,
+    ) -> blockchain_models.UnbindCaasApplicationManageResponse:
+        """
+        Description: 解除授权
+        Summary: 解除授权
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.unbind_caas_application_manage_ex_async(request, headers, runtime)
+
+    def unbind_caas_application_manage_ex(
+        self,
+        request: blockchain_models.UnbindCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.UnbindCaasApplicationManageResponse:
+        """
+        Description: 解除授权
+        Summary: 解除授权
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.UnbindCaasApplicationManageResponse(),
+            self.do_request('1.0', 'baas.caas.application.manage.unbind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def unbind_caas_application_manage_ex_async(
+        self,
+        request: blockchain_models.UnbindCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.UnbindCaasApplicationManageResponse:
+        """
+        Description: 解除授权
+        Summary: 解除授权
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.UnbindCaasApplicationManageResponse(),
+            await self.do_request_async('1.0', 'baas.caas.application.manage.unbind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def bind_caas_application_manage(
+        self,
+        request: blockchain_models.BindCaasApplicationManageRequest,
+    ) -> blockchain_models.BindCaasApplicationManageResponse:
+        """
+        Description: 绑定合约
+        Summary: 绑定合约
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.bind_caas_application_manage_ex(request, headers, runtime)
+
+    async def bind_caas_application_manage_async(
+        self,
+        request: blockchain_models.BindCaasApplicationManageRequest,
+    ) -> blockchain_models.BindCaasApplicationManageResponse:
+        """
+        Description: 绑定合约
+        Summary: 绑定合约
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.bind_caas_application_manage_ex_async(request, headers, runtime)
+
+    def bind_caas_application_manage_ex(
+        self,
+        request: blockchain_models.BindCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.BindCaasApplicationManageResponse:
+        """
+        Description: 绑定合约
+        Summary: 绑定合约
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.BindCaasApplicationManageResponse(),
+            self.do_request('1.0', 'baas.caas.application.manage.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def bind_caas_application_manage_ex_async(
+        self,
+        request: blockchain_models.BindCaasApplicationManageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.BindCaasApplicationManageResponse:
+        """
+        Description: 绑定合约
+        Summary: 绑定合约
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.BindCaasApplicationManageResponse(),
+            await self.do_request_async('1.0', 'baas.caas.application.manage.bind', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def delete_caas_contract_service(
+        self,
+        request: blockchain_models.DeleteCaasContractServiceRequest,
+    ) -> blockchain_models.DeleteCaasContractServiceResponse:
+        """
+        Description: 删除合约
+        Summary: 删除合约
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.delete_caas_contract_service_ex(request, headers, runtime)
+
+    async def delete_caas_contract_service_async(
+        self,
+        request: blockchain_models.DeleteCaasContractServiceRequest,
+    ) -> blockchain_models.DeleteCaasContractServiceResponse:
+        """
+        Description: 删除合约
+        Summary: 删除合约
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.delete_caas_contract_service_ex_async(request, headers, runtime)
+
+    def delete_caas_contract_service_ex(
+        self,
+        request: blockchain_models.DeleteCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.DeleteCaasContractServiceResponse:
+        """
+        Description: 删除合约
+        Summary: 删除合约
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.DeleteCaasContractServiceResponse(),
+            self.do_request('1.0', 'baas.caas.contract.service.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def delete_caas_contract_service_ex_async(
+        self,
+        request: blockchain_models.DeleteCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.DeleteCaasContractServiceResponse:
+        """
+        Description: 删除合约
+        Summary: 删除合约
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.DeleteCaasContractServiceResponse(),
+            await self.do_request_async('1.0', 'baas.caas.contract.service.delete', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def create_caas_contract_service(
+        self,
+        request: blockchain_models.CreateCaasContractServiceRequest,
+    ) -> blockchain_models.CreateCaasContractServiceResponse:
+        """
+        Description: 新建合约服务
+        Summary: 新建合约服务
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_caas_contract_service_ex(request, headers, runtime)
+
+    async def create_caas_contract_service_async(
+        self,
+        request: blockchain_models.CreateCaasContractServiceRequest,
+    ) -> blockchain_models.CreateCaasContractServiceResponse:
+        """
+        Description: 新建合约服务
+        Summary: 新建合约服务
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_caas_contract_service_ex_async(request, headers, runtime)
+
+    def create_caas_contract_service_ex(
+        self,
+        request: blockchain_models.CreateCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.CreateCaasContractServiceResponse:
+        """
+        Description: 新建合约服务
+        Summary: 新建合约服务
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.CreateCaasContractServiceResponse(),
+            self.do_request('1.0', 'baas.caas.contract.service.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def create_caas_contract_service_ex_async(
+        self,
+        request: blockchain_models.CreateCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.CreateCaasContractServiceResponse:
+        """
+        Description: 新建合约服务
+        Summary: 新建合约服务
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.CreateCaasContractServiceResponse(),
+            await self.do_request_async('1.0', 'baas.caas.contract.service.create', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_caas_contract_service(
+        self,
+        request: blockchain_models.PagequeryCaasContractServiceRequest,
+    ) -> blockchain_models.PagequeryCaasContractServiceResponse:
+        """
+        Description: 我的合约列表查询
+        Summary: 我的合约列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_caas_contract_service_ex(request, headers, runtime)
+
+    async def pagequery_caas_contract_service_async(
+        self,
+        request: blockchain_models.PagequeryCaasContractServiceRequest,
+    ) -> blockchain_models.PagequeryCaasContractServiceResponse:
+        """
+        Description: 我的合约列表查询
+        Summary: 我的合约列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_caas_contract_service_ex_async(request, headers, runtime)
+
+    def pagequery_caas_contract_service_ex(
+        self,
+        request: blockchain_models.PagequeryCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.PagequeryCaasContractServiceResponse:
+        """
+        Description: 我的合约列表查询
+        Summary: 我的合约列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.PagequeryCaasContractServiceResponse(),
+            self.do_request('1.0', 'baas.caas.contract.service.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_caas_contract_service_ex_async(
+        self,
+        request: blockchain_models.PagequeryCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.PagequeryCaasContractServiceResponse:
+        """
+        Description: 我的合约列表查询
+        Summary: 我的合约列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.PagequeryCaasContractServiceResponse(),
+            await self.do_request_async('1.0', 'baas.caas.contract.service.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def list_caas_contract_service(
+        self,
+        request: blockchain_models.ListCaasContractServiceRequest,
+    ) -> blockchain_models.ListCaasContractServiceResponse:
+        """
+        Description: 查询合约类型列表
+        Summary: 查询合约类型列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_caas_contract_service_ex(request, headers, runtime)
+
+    async def list_caas_contract_service_async(
+        self,
+        request: blockchain_models.ListCaasContractServiceRequest,
+    ) -> blockchain_models.ListCaasContractServiceResponse:
+        """
+        Description: 查询合约类型列表
+        Summary: 查询合约类型列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_caas_contract_service_ex_async(request, headers, runtime)
+
+    def list_caas_contract_service_ex(
+        self,
+        request: blockchain_models.ListCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.ListCaasContractServiceResponse:
+        """
+        Description: 查询合约类型列表
+        Summary: 查询合约类型列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.ListCaasContractServiceResponse(),
+            self.do_request('1.0', 'baas.caas.contract.service.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def list_caas_contract_service_ex_async(
+        self,
+        request: blockchain_models.ListCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.ListCaasContractServiceResponse:
+        """
+        Description: 查询合约类型列表
+        Summary: 查询合约类型列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.ListCaasContractServiceResponse(),
+            await self.do_request_async('1.0', 'baas.caas.contract.service.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def deploy_caas_contract_service(
+        self,
+        request: blockchain_models.DeployCaasContractServiceRequest,
+    ) -> blockchain_models.DeployCaasContractServiceResponse:
+        """
+        Description: 自动化部署合约服务（合约部署 + 应用创建 + 应用合约授权）
+        Summary: 自动化部署合约服务（合约部署 + 应用创建 + 应用合约授权）
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.deploy_caas_contract_service_ex(request, headers, runtime)
+
+    async def deploy_caas_contract_service_async(
+        self,
+        request: blockchain_models.DeployCaasContractServiceRequest,
+    ) -> blockchain_models.DeployCaasContractServiceResponse:
+        """
+        Description: 自动化部署合约服务（合约部署 + 应用创建 + 应用合约授权）
+        Summary: 自动化部署合约服务（合约部署 + 应用创建 + 应用合约授权）
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.deploy_caas_contract_service_ex_async(request, headers, runtime)
+
+    def deploy_caas_contract_service_ex(
+        self,
+        request: blockchain_models.DeployCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.DeployCaasContractServiceResponse:
+        """
+        Description: 自动化部署合约服务（合约部署 + 应用创建 + 应用合约授权）
+        Summary: 自动化部署合约服务（合约部署 + 应用创建 + 应用合约授权）
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.DeployCaasContractServiceResponse(),
+            self.do_request('1.0', 'baas.caas.contract.service.deploy', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def deploy_caas_contract_service_ex_async(
+        self,
+        request: blockchain_models.DeployCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.DeployCaasContractServiceResponse:
+        """
+        Description: 自动化部署合约服务（合约部署 + 应用创建 + 应用合约授权）
+        Summary: 自动化部署合约服务（合约部署 + 应用创建 + 应用合约授权）
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.DeployCaasContractServiceResponse(),
+            await self.do_request_async('1.0', 'baas.caas.contract.service.deploy', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def detail_caas_contract_service(
+        self,
+        request: blockchain_models.DetailCaasContractServiceRequest,
+    ) -> blockchain_models.DetailCaasContractServiceResponse:
+        """
+        Description: 合约详情
+        Summary: 合约详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.detail_caas_contract_service_ex(request, headers, runtime)
+
+    async def detail_caas_contract_service_async(
+        self,
+        request: blockchain_models.DetailCaasContractServiceRequest,
+    ) -> blockchain_models.DetailCaasContractServiceResponse:
+        """
+        Description: 合约详情
+        Summary: 合约详情
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.detail_caas_contract_service_ex_async(request, headers, runtime)
+
+    def detail_caas_contract_service_ex(
+        self,
+        request: blockchain_models.DetailCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.DetailCaasContractServiceResponse:
+        """
+        Description: 合约详情
+        Summary: 合约详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.DetailCaasContractServiceResponse(),
+            self.do_request('1.0', 'baas.caas.contract.service.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def detail_caas_contract_service_ex_async(
+        self,
+        request: blockchain_models.DetailCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.DetailCaasContractServiceResponse:
+        """
+        Description: 合约详情
+        Summary: 合约详情
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.DetailCaasContractServiceResponse(),
+            await self.do_request_async('1.0', 'baas.caas.contract.service.detail', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_caas_contract_service(
+        self,
+        request: blockchain_models.QueryCaasContractServiceRequest,
+    ) -> blockchain_models.QueryCaasContractServiceResponse:
+        """
+        Description: 查询创建实例进度
+        Summary: 查询创建实例进度
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_caas_contract_service_ex(request, headers, runtime)
+
+    async def query_caas_contract_service_async(
+        self,
+        request: blockchain_models.QueryCaasContractServiceRequest,
+    ) -> blockchain_models.QueryCaasContractServiceResponse:
+        """
+        Description: 查询创建实例进度
+        Summary: 查询创建实例进度
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_caas_contract_service_ex_async(request, headers, runtime)
+
+    def query_caas_contract_service_ex(
+        self,
+        request: blockchain_models.QueryCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.QueryCaasContractServiceResponse:
+        """
+        Description: 查询创建实例进度
+        Summary: 查询创建实例进度
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.QueryCaasContractServiceResponse(),
+            self.do_request('1.0', 'baas.caas.contract.service.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_caas_contract_service_ex_async(
+        self,
+        request: blockchain_models.QueryCaasContractServiceRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.QueryCaasContractServiceResponse:
+        """
+        Description: 查询创建实例进度
+        Summary: 查询创建实例进度
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.QueryCaasContractServiceResponse(),
+            await self.do_request_async('1.0', 'baas.caas.contract.service.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def pagequery_caas_contract_market(
+        self,
+        request: blockchain_models.PagequeryCaasContractMarketRequest,
+    ) -> blockchain_models.PagequeryCaasContractMarketResponse:
+        """
+        Description: 智能合约市场列表查询
+        Summary: 智能合约市场列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.pagequery_caas_contract_market_ex(request, headers, runtime)
+
+    async def pagequery_caas_contract_market_async(
+        self,
+        request: blockchain_models.PagequeryCaasContractMarketRequest,
+    ) -> blockchain_models.PagequeryCaasContractMarketResponse:
+        """
+        Description: 智能合约市场列表查询
+        Summary: 智能合约市场列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.pagequery_caas_contract_market_ex_async(request, headers, runtime)
+
+    def pagequery_caas_contract_market_ex(
+        self,
+        request: blockchain_models.PagequeryCaasContractMarketRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.PagequeryCaasContractMarketResponse:
+        """
+        Description: 智能合约市场列表查询
+        Summary: 智能合约市场列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.PagequeryCaasContractMarketResponse(),
+            self.do_request('1.0', 'baas.caas.contract.market.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def pagequery_caas_contract_market_ex_async(
+        self,
+        request: blockchain_models.PagequeryCaasContractMarketRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.PagequeryCaasContractMarketResponse:
+        """
+        Description: 智能合约市场列表查询
+        Summary: 智能合约市场列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.PagequeryCaasContractMarketResponse(),
+            await self.do_request_async('1.0', 'baas.caas.contract.market.pagequery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_contract_record(
         self,
         request: blockchain_models.CreateContractRecordRequest,
     ) -> blockchain_models.CreateContractRecordResponse:
         """
         Description: 合约部署记录
         Summary: 合约部署记录
@@ -21379,14 +22163,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             blockchain_models.QueryAuthCertDetailurlResponse(),
             await self.do_request_async('1.0', 'baas.auth.cert.detailurl.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def notify_auth_task_status(
+        self,
+        request: blockchain_models.NotifyAuthTaskStatusRequest,
+    ) -> blockchain_models.NotifyAuthTaskStatusResponse:
+        """
+        Description: 主站应用同步授权宝权益任务的完成情况
+        Summary: 主站应用同步授权宝权益任务的完成情况
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.notify_auth_task_status_ex(request, headers, runtime)
+
+    async def notify_auth_task_status_async(
+        self,
+        request: blockchain_models.NotifyAuthTaskStatusRequest,
+    ) -> blockchain_models.NotifyAuthTaskStatusResponse:
+        """
+        Description: 主站应用同步授权宝权益任务的完成情况
+        Summary: 主站应用同步授权宝权益任务的完成情况
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.notify_auth_task_status_ex_async(request, headers, runtime)
+
+    def notify_auth_task_status_ex(
+        self,
+        request: blockchain_models.NotifyAuthTaskStatusRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.NotifyAuthTaskStatusResponse:
+        """
+        Description: 主站应用同步授权宝权益任务的完成情况
+        Summary: 主站应用同步授权宝权益任务的完成情况
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.NotifyAuthTaskStatusResponse(),
+            self.do_request('1.0', 'baas.auth.task.status.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def notify_auth_task_status_ex_async(
+        self,
+        request: blockchain_models.NotifyAuthTaskStatusRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.NotifyAuthTaskStatusResponse:
+        """
+        Description: 主站应用同步授权宝权益任务的完成情况
+        Summary: 主站应用同步授权宝权益任务的完成情况
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.NotifyAuthTaskStatusResponse(),
+            await self.do_request_async('1.0', 'baas.auth.task.status.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def start_did_corporate_agentcreate(
         self,
         request: blockchain_models.StartDidCorporateAgentcreateRequest,
     ) -> blockchain_models.StartDidCorporateAgentcreateResponse:
         """
         Description: 通过代理模式为企业创建did
         Summary: 通过代理模式为企业创建did
```

### Comparing `antchain_blockchain-1.26.33/antchain_sdk_blockchain/models.py` & `antchain_blockchain-1.26.36/antchain_sdk_blockchain/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1017,14 +1017,63 @@
         if m.get('type') is not None:
             self.type = m.get('type')
         if m.get('desc') is not None:
             self.desc = m.get('desc')
         return self
 
 
+class ContractListResp(TeaModel):
+    def __init__(
+        self,
+        service_id: str = None,
+        name: str = None,
+        type: str = None,
+        create_time: int = None,
+    ):
+        # 服务ID
+        self.service_id = service_id
+        # 合约名称
+        self.name = name
+        # 合约类型
+        self.type = type
+        # 创建时间
+        self.create_time = create_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.service_id is not None:
+            result['service_id'] = self.service_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.type is not None:
+            result['type'] = self.type
+        if self.create_time is not None:
+            result['create_time'] = self.create_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('service_id') is not None:
+            self.service_id = m.get('service_id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('create_time') is not None:
+            self.create_time = m.get('create_time')
+        return self
+
+
 class ALiYunContractBlockchain(TeaModel):
     def __init__(
         self,
         name: str = None,
         bizid: str = None,
         chain_type: str = None,
         node_num: int = None,
@@ -1101,14 +1150,77 @@
         if m.get('network') is not None:
             self.network = m.get('network')
         if m.get('version') is not None:
             self.version = m.get('version')
         return self
 
 
+class InstanceProgressInfo(TeaModel):
+    def __init__(
+        self,
+        operator: str = None,
+        time: int = None,
+        type: str = None,
+        status: str = None,
+        type_name: str = None,
+        data: str = None,
+    ):
+        # 操作人
+        self.operator = operator
+        # 操作时间
+        self.time = time
+        # 合约部署进度类型
+        self.type = type
+        # 部署状态
+        self.status = status
+        # 合约部署进度名称
+        self.type_name = type_name
+        # 额外参数
+        self.data = data
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.operator is not None:
+            result['operator'] = self.operator
+        if self.time is not None:
+            result['time'] = self.time
+        if self.type is not None:
+            result['type'] = self.type
+        if self.status is not None:
+            result['status'] = self.status
+        if self.type_name is not None:
+            result['type_name'] = self.type_name
+        if self.data is not None:
+            result['data'] = self.data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('operator') is not None:
+            self.operator = m.get('operator')
+        if m.get('time') is not None:
+            self.time = m.get('time')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('type_name') is not None:
+            self.type_name = m.get('type_name')
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
 class ALiYunChainMiniAppAuthorizedUser(TeaModel):
     def __init__(
         self,
         phone: str = None,
         gmt_authorized: str = None,
         user_id: int = None,
     ):
@@ -2159,14 +2271,56 @@
         if m.get('to') is not None:
             self.to = m.get('to')
         if m.get('gas_used') is not None:
             self.gas_used = m.get('gas_used')
         return self
 
 
+class InstanceRecordInfo(TeaModel):
+    def __init__(
+        self,
+        application: str = None,
+        status: str = None,
+        operating_time: str = None,
+    ):
+        # 应用标识
+        self.application = application
+        # 执行结果
+        self.status = status
+        # 操作时间
+        self.operating_time = operating_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.application is not None:
+            result['application'] = self.application
+        if self.status is not None:
+            result['status'] = self.status
+        if self.operating_time is not None:
+            result['operating_time'] = self.operating_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('application') is not None:
+            self.application = m.get('application')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('operating_time') is not None:
+            self.operating_time = m.get('operating_time')
+        return self
+
+
 class ALiYunAccount(TeaModel):
     def __init__(
         self,
         ant_chain_id: str = None,
         account: str = None,
         account_public_key: str = None,
         account_recovery_key: str = None,
@@ -2540,14 +2694,56 @@
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('uid') is not None:
             self.uid = m.get('uid')
         return self
 
 
+class ApplicationListResp(TeaModel):
+    def __init__(
+        self,
+        application_id: str = None,
+        access_key: str = None,
+        name_list: List[str] = None,
+    ):
+        # 应用程序ID
+        self.application_id = application_id
+        # 链ID
+        self.access_key = access_key
+        # 合约(创建实例时填写的合约名称。)
+        self.name_list = name_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.application_id is not None:
+            result['application_id'] = self.application_id
+        if self.access_key is not None:
+            result['access_key'] = self.access_key
+        if self.name_list is not None:
+            result['name_list'] = self.name_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('application_id') is not None:
+            self.application_id = m.get('application_id')
+        if m.get('access_key') is not None:
+            self.access_key = m.get('access_key')
+        if m.get('name_list') is not None:
+            self.name_list = m.get('name_list')
+        return self
+
+
 class VcTransmitTargetStruct(TeaModel):
     def __init__(
         self,
         public_key: str = None,
         vc_channel: str = None,
         verifier_did: str = None,
     ):
@@ -4901,14 +5097,42 @@
         if m.get('issuer_id') is not None:
             self.issuer_id = m.get('issuer_id')
         if m.get('recipient_id') is not None:
             self.recipient_id = m.get('recipient_id')
         return self
 
 
+class ContractTypeResp(TeaModel):
+    def __init__(
+        self,
+        type: str = None,
+    ):
+        # 合约服务类型
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
 class LogisticLocation(TeaModel):
     def __init__(
         self,
         address: str = None,
         city_code: str = None,
         lat: str = None,
         lon: str = None,
@@ -5659,14 +5883,57 @@
         if m.get('result') is not None:
             self.result = m.get('result')
         if m.get('logs') is not None:
             self.logs = m.get('logs')
         return self
 
 
+class ContractCreateProcessResp(TeaModel):
+    def __init__(
+        self,
+        status: str = None,
+        progress_info_list: List[InstanceProgressInfo] = None,
+    ):
+        # 当前进度信息
+        self.status = status
+        # 合约部署进度
+        self.progress_info_list = progress_info_list
+
+    def validate(self):
+        if self.progress_info_list:
+            for k in self.progress_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.status is not None:
+            result['status'] = self.status
+        result['progress_info_list'] = []
+        if self.progress_info_list is not None:
+            for k in self.progress_info_list:
+                result['progress_info_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        self.progress_info_list = []
+        if m.get('progress_info_list') is not None:
+            for k in m.get('progress_info_list'):
+                temp_model = InstanceProgressInfo()
+                self.progress_info_list.append(temp_model.from_map(k))
+        return self
+
+
 class ProcessResult(TeaModel):
     def __init__(
         self,
         extension: str = None,
         message: str = None,
         next: str = None,
         process_id: str = None,
@@ -6669,14 +6936,57 @@
         if m.get('phone_number') is not None:
             self.phone_number = m.get('phone_number')
         if m.get('user_name') is not None:
             self.user_name = m.get('user_name')
         return self
 
 
+class PageRespApplicationListResp(TeaModel):
+    def __init__(
+        self,
+        total: int = None,
+        data_list: List[ApplicationListResp] = None,
+    ):
+        # 总数
+        self.total = total
+        # 列表数据
+        self.data_list = data_list
+
+    def validate(self):
+        if self.data_list:
+            for k in self.data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.total is not None:
+            result['total'] = self.total
+        result['data_list'] = []
+        if self.data_list is not None:
+            for k in self.data_list:
+                result['data_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        self.data_list = []
+        if m.get('data_list') is not None:
+            for k in m.get('data_list'):
+                temp_model = ApplicationListResp()
+                self.data_list.append(temp_model.from_map(k))
+        return self
+
+
 class AccountInfoWithBiz(TeaModel):
     def __init__(
         self,
         address: str = None,
         biz_code: str = None,
         biz_name: str = None,
         biz_type: str = None,
@@ -7128,14 +7438,57 @@
         if m.get('consortium_name') is not None:
             self.consortium_name = m.get('consortium_name')
         if m.get('consortium_id') is not None:
             self.consortium_id = m.get('consortium_id')
         return self
 
 
+class PageRespContractListResp(TeaModel):
+    def __init__(
+        self,
+        total: int = None,
+        data_list: List[ContractListResp] = None,
+    ):
+        # 总数
+        self.total = total
+        # 列表数据
+        self.data_list = data_list
+
+    def validate(self):
+        if self.data_list:
+            for k in self.data_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.total is not None:
+            result['total'] = self.total
+        result['data_list'] = []
+        if self.data_list is not None:
+            for k in self.data_list:
+                result['data_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        self.data_list = []
+        if m.get('data_list') is not None:
+            for k in m.get('data_list'):
+                temp_model = ContractListResp()
+                self.data_list.append(temp_model.from_map(k))
+        return self
+
+
 class VcShareStruct(TeaModel):
     def __init__(
         self,
         vc_id: str = None,
         owner_did: str = None,
         index: str = None,
         signature: str = None,
@@ -8469,14 +8822,78 @@
         if m.get('last_sum_block_height') is not None:
             self.last_sum_block_height = m.get('last_sum_block_height')
         if m.get('creat_time') is not None:
             self.creat_time = m.get('creat_time')
         return self
 
 
+class EWRFW(TeaModel):
+    def __init__(
+        self,
+        sdf: List[DidDocServicesInfo] = None,
+        www: str = None,
+        list_string: List[str] = None,
+        aaa: DidDocServicesInfo = None,
+    ):
+        # FFF
+        self.sdf = sdf
+        # www
+        self.www = www
+        # ss
+        self.list_string = list_string
+        # aaa
+        self.aaa = aaa
+
+    def validate(self):
+        self.validate_required(self.sdf, 'sdf')
+        if self.sdf:
+            for k in self.sdf:
+                if k:
+                    k.validate()
+        self.validate_required(self.www, 'www')
+        self.validate_required(self.list_string, 'list_string')
+        self.validate_required(self.aaa, 'aaa')
+        if self.aaa:
+            self.aaa.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['sdf'] = []
+        if self.sdf is not None:
+            for k in self.sdf:
+                result['sdf'].append(k.to_map() if k else None)
+        if self.www is not None:
+            result['www'] = self.www
+        if self.list_string is not None:
+            result['list_string'] = self.list_string
+        if self.aaa is not None:
+            result['aaa'] = self.aaa.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.sdf = []
+        if m.get('sdf') is not None:
+            for k in m.get('sdf'):
+                temp_model = DidDocServicesInfo()
+                self.sdf.append(temp_model.from_map(k))
+        if m.get('www') is not None:
+            self.www = m.get('www')
+        if m.get('list_string') is not None:
+            self.list_string = m.get('list_string')
+        if m.get('aaa') is not None:
+            temp_model = DidDocServicesInfo()
+            self.aaa = temp_model.from_map(m['aaa'])
+        return self
+
+
 class ALiYunCertificateApplications(TeaModel):
     def __init__(
         self,
         pagination: ALiYunPagination = None,
         certificate_applications: List[ALiYunCertificateApplication] = None,
     ):
         # pagination
@@ -9084,14 +9501,56 @@
         if m.get('hash') is not None:
             self.hash = m.get('hash')
         if m.get('timestamp') is not None:
             self.timestamp = m.get('timestamp')
         return self
 
 
+class ContractBindAppResp(TeaModel):
+    def __init__(
+        self,
+        service_id: str = None,
+        name: str = None,
+        bind: bool = None,
+    ):
+        # 合约标识
+        self.service_id = service_id
+        # 合约名称
+        self.name = name
+        # 是否已关联
+        self.bind = bind
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.service_id is not None:
+            result['service_id'] = self.service_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.bind is not None:
+            result['bind'] = self.bind
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('service_id') is not None:
+            self.service_id = m.get('service_id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('bind') is not None:
+            self.bind = m.get('bind')
+        return self
+
+
 class AddVC(TeaModel):
     def __init__(
         self,
         content_hash: str = None,
         issuer_hash: str = None,
         status: str = None,
         subject_hash: str = None,
@@ -9144,14 +9603,122 @@
         if m.get('subject_hash') is not None:
             self.subject_hash = m.get('subject_hash')
         if m.get('vc_id') is not None:
             self.vc_id = m.get('vc_id')
         return self
 
 
+class ContractDetailResp(TeaModel):
+    def __init__(
+        self,
+        service_id: str = None,
+        name: str = None,
+        creator: str = None,
+        create_time: int = None,
+        ordering_products: str = None,
+        chan_id: str = None,
+        contract_status: str = None,
+        status: str = None,
+        progress_info_list: List[InstanceProgressInfo] = None,
+        record_info_list: List[InstanceRecordInfo] = None,
+    ):
+        # 合约标识
+        self.service_id = service_id
+        # 合约服务名称
+        self.name = name
+        # 创建人
+        self.creator = creator
+        # 创建时间
+        self.create_time = create_time
+        # 订购产品
+        self.ordering_products = ordering_products
+        # 关联区块链id
+        self.chan_id = chan_id
+        # 合约状态
+        self.contract_status = contract_status
+        # 合约部署进度当前状态
+        self.status = status
+        # 合约部署进度
+        self.progress_info_list = progress_info_list
+        # 实例最近调用记录(暂缓，先不做)
+        self.record_info_list = record_info_list
+
+    def validate(self):
+        if self.progress_info_list:
+            for k in self.progress_info_list:
+                if k:
+                    k.validate()
+        if self.record_info_list:
+            for k in self.record_info_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.service_id is not None:
+            result['service_id'] = self.service_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.creator is not None:
+            result['creator'] = self.creator
+        if self.create_time is not None:
+            result['create_time'] = self.create_time
+        if self.ordering_products is not None:
+            result['ordering_products'] = self.ordering_products
+        if self.chan_id is not None:
+            result['chan_id'] = self.chan_id
+        if self.contract_status is not None:
+            result['contract_status'] = self.contract_status
+        if self.status is not None:
+            result['status'] = self.status
+        result['progress_info_list'] = []
+        if self.progress_info_list is not None:
+            for k in self.progress_info_list:
+                result['progress_info_list'].append(k.to_map() if k else None)
+        result['record_info_list'] = []
+        if self.record_info_list is not None:
+            for k in self.record_info_list:
+                result['record_info_list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('service_id') is not None:
+            self.service_id = m.get('service_id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('creator') is not None:
+            self.creator = m.get('creator')
+        if m.get('create_time') is not None:
+            self.create_time = m.get('create_time')
+        if m.get('ordering_products') is not None:
+            self.ordering_products = m.get('ordering_products')
+        if m.get('chan_id') is not None:
+            self.chan_id = m.get('chan_id')
+        if m.get('contract_status') is not None:
+            self.contract_status = m.get('contract_status')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        self.progress_info_list = []
+        if m.get('progress_info_list') is not None:
+            for k in m.get('progress_info_list'):
+                temp_model = InstanceProgressInfo()
+                self.progress_info_list.append(temp_model.from_map(k))
+        self.record_info_list = []
+        if m.get('record_info_list') is not None:
+            for k in m.get('record_info_list'):
+                temp_model = InstanceRecordInfo()
+                self.record_info_list.append(temp_model.from_map(k))
+        return self
+
+
 class ValueUnitPair(TeaModel):
     def __init__(
         self,
         value: int = None,
         unit: str = None,
     ):
         # 数值
@@ -9963,14 +10530,42 @@
         if m.get('title') is not None:
             self.title = m.get('title')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
 
 
+class ContractListReq(TeaModel):
+    def __init__(
+        self,
+        type: str = None,
+    ):
+        # 合约服务类别
+        self.type = type
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
 class TappInfo(TeaModel):
     def __init__(
         self,
         taap_id: str = None,
         tapp_version: int = None,
     ):
         # C3S可信计算TAPP应用标识
@@ -10644,14 +11239,77 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('doc') is not None:
             self.doc = m.get('doc')
         return self
 
 
+class ContractTemplateResp(TeaModel):
+    def __init__(
+        self,
+        template_id: str = None,
+        name: str = None,
+        thumb_url: str = None,
+        description: str = None,
+        open: bool = None,
+        avatar_logo_list: List[str] = None,
+    ):
+        # 模板标识
+        self.template_id = template_id
+        # 合约名称
+        self.name = name
+        # 缩略图url
+        self.thumb_url = thumb_url
+        # 合约描述
+        self.description = description
+        # 是否已开通合约
+        self.open = open
+        # 后续展示：购买用户头像
+        self.avatar_logo_list = avatar_logo_list
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.template_id is not None:
+            result['template_id'] = self.template_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.thumb_url is not None:
+            result['thumb_url'] = self.thumb_url
+        if self.description is not None:
+            result['description'] = self.description
+        if self.open is not None:
+            result['open'] = self.open
+        if self.avatar_logo_list is not None:
+            result['avatar_logo_list'] = self.avatar_logo_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('template_id') is not None:
+            self.template_id = m.get('template_id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('thumb_url') is not None:
+            self.thumb_url = m.get('thumb_url')
+        if m.get('description') is not None:
+            self.description = m.get('description')
+        if m.get('open') is not None:
+            self.open = m.get('open')
+        if m.get('avatar_logo_list') is not None:
+            self.avatar_logo_list = m.get('avatar_logo_list')
+        return self
+
+
 class TemplateInfoDTO(TeaModel):
     def __init__(
         self,
         id: int = None,
         category: str = None,
         claim_template: str = None,
         gmt_create: str = None,
@@ -40319,14 +40977,1721 @@
         if m.get('transaction_list') is not None:
             for k in m.get('transaction_list'):
                 temp_model = TransactionInfo()
                 self.transaction_list.append(temp_model.from_map(k))
         return self
 
 
+class CreateCaasApplicationManageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class CreateCaasApplicationManageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        application_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 应用id
+        self.application_id = application_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.application_id is not None:
+            result['application_id'] = self.application_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('application_id') is not None:
+            self.application_id = m.get('application_id')
+        return self
+
+
+class PagequeryCaasApplicationManageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        num: int = None,
+        size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 页码
+        self.num = num
+        # 页大小
+        self.size = size
+
+    def validate(self):
+        self.validate_required(self.num, 'num')
+        self.validate_required(self.size, 'size')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.num is not None:
+            result['num'] = self.num
+        if self.size is not None:
+            result['size'] = self.size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('num') is not None:
+            self.num = m.get('num')
+        if m.get('size') is not None:
+            self.size = m.get('size')
+        return self
+
+
+class PagequeryCaasApplicationManageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        data: PageRespApplicationListResp = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 请求结果数据
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('data') is not None:
+            temp_model = PageRespApplicationListResp()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
+class GetCaasApplicationManageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        application_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 应用程序ID
+        self.application_id = application_id
+
+    def validate(self):
+        self.validate_required(self.application_id, 'application_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.application_id is not None:
+            result['application_id'] = self.application_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('application_id') is not None:
+            self.application_id = m.get('application_id')
+        return self
+
+
+class GetCaasApplicationManageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 应用秘钥
+        self.data = data
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.data is not None:
+            result['data'] = self.data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class QueryCaasApplicationManageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        application_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 应用程序ID
+        self.application_id = application_id
+
+    def validate(self):
+        self.validate_required(self.application_id, 'application_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.application_id is not None:
+            result['application_id'] = self.application_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('application_id') is not None:
+            self.application_id = m.get('application_id')
+        return self
+
+
+class QueryCaasApplicationManageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        data: List[ContractBindAppResp] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 请求结果数据
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        result['data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['data'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        self.data = []
+        if m.get('data') is not None:
+            for k in m.get('data'):
+                temp_model = ContractBindAppResp()
+                self.data.append(temp_model.from_map(k))
+        return self
+
+
+class UnbindCaasApplicationManageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        application_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 应用程序ID
+        self.application_id = application_id
+
+    def validate(self):
+        self.validate_required(self.application_id, 'application_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.application_id is not None:
+            result['application_id'] = self.application_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('application_id') is not None:
+            self.application_id = m.get('application_id')
+        return self
+
+
+class UnbindCaasApplicationManageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        return self
+
+
+class BindCaasApplicationManageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        application_id: str = None,
+        service_ids: List[str] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 应用程序ID
+        self.application_id = application_id
+        # 合约服务标识集合
+        self.service_ids = service_ids
+
+    def validate(self):
+        self.validate_required(self.application_id, 'application_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.application_id is not None:
+            result['application_id'] = self.application_id
+        if self.service_ids is not None:
+            result['service_ids'] = self.service_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('application_id') is not None:
+            self.application_id = m.get('application_id')
+        if m.get('service_ids') is not None:
+            self.service_ids = m.get('service_ids')
+        return self
+
+
+class BindCaasApplicationManageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        return self
+
+
+class DeleteCaasContractServiceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        service_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 服务ID
+        self.service_id = service_id
+
+    def validate(self):
+        self.validate_required(self.service_id, 'service_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.service_id is not None:
+            result['service_id'] = self.service_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('service_id') is not None:
+            self.service_id = m.get('service_id')
+        return self
+
+
+class DeleteCaasContractServiceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        return self
+
+
+class CreateCaasContractServiceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        chain_id: str = None,
+        template_id: str = None,
+        name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 链ID
+        self.chain_id = chain_id
+        # 合约模板标识
+        self.template_id = template_id
+        # 合约名称
+        self.name = name
+
+    def validate(self):
+        self.validate_required(self.chain_id, 'chain_id')
+        self.validate_required(self.template_id, 'template_id')
+        self.validate_required(self.name, 'name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.chain_id is not None:
+            result['chain_id'] = self.chain_id
+        if self.template_id is not None:
+            result['template_id'] = self.template_id
+        if self.name is not None:
+            result['name'] = self.name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('chain_id') is not None:
+            self.chain_id = m.get('chain_id')
+        if m.get('template_id') is not None:
+            self.template_id = m.get('template_id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        return self
+
+
+class CreateCaasContractServiceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 请求结果数据
+        self.data = data
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.data is not None:
+            result['data'] = self.data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class PagequeryCaasContractServiceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        num: int = None,
+        size: int = None,
+        data: ContractListReq = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 页码
+        self.num = num
+        # 页大小
+        self.size = size
+        # 业务数据
+        self.data = data
+
+    def validate(self):
+        self.validate_required(self.num, 'num')
+        self.validate_required(self.size, 'size')
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.num is not None:
+            result['num'] = self.num
+        if self.size is not None:
+            result['size'] = self.size
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('num') is not None:
+            self.num = m.get('num')
+        if m.get('size') is not None:
+            self.size = m.get('size')
+        if m.get('data') is not None:
+            temp_model = ContractListReq()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
+class PagequeryCaasContractServiceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        data: PageRespContractListResp = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 请求结果数据
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('data') is not None:
+            temp_model = PageRespContractListResp()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
+class ListCaasContractServiceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class ListCaasContractServiceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        data: List[ContractTypeResp] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 请求结果数据
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        result['data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['data'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        self.data = []
+        if m.get('data') is not None:
+            for k in m.get('data'):
+                temp_model = ContractTypeResp()
+                self.data.append(temp_model.from_map(k))
+        return self
+
+
+class DeployCaasContractServiceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        chain_id: str = None,
+        template_id: str = None,
+        name: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 链ID
+        self.chain_id = chain_id
+        # 合约模板标识
+        self.template_id = template_id
+        # 合约名称
+        self.name = name
+
+    def validate(self):
+        self.validate_required(self.chain_id, 'chain_id')
+        self.validate_required(self.template_id, 'template_id')
+        self.validate_required(self.name, 'name')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.chain_id is not None:
+            result['chain_id'] = self.chain_id
+        if self.template_id is not None:
+            result['template_id'] = self.template_id
+        if self.name is not None:
+            result['name'] = self.name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('chain_id') is not None:
+            self.chain_id = m.get('chain_id')
+        if m.get('template_id') is not None:
+            self.template_id = m.get('template_id')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        return self
+
+
+class DeployCaasContractServiceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        data: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 请求结果数据
+        self.data = data
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.data is not None:
+            result['data'] = self.data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('data') is not None:
+            self.data = m.get('data')
+        return self
+
+
+class DetailCaasContractServiceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        service_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 服务ID
+        self.service_id = service_id
+
+    def validate(self):
+        self.validate_required(self.service_id, 'service_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.service_id is not None:
+            result['service_id'] = self.service_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('service_id') is not None:
+            self.service_id = m.get('service_id')
+        return self
+
+
+class DetailCaasContractServiceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        data: ContractDetailResp = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 请求结果数据
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('data') is not None:
+            temp_model = ContractDetailResp()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
+class QueryCaasContractServiceRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        service_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 服务ID
+        self.service_id = service_id
+
+    def validate(self):
+        self.validate_required(self.service_id, 'service_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.service_id is not None:
+            result['service_id'] = self.service_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('service_id') is not None:
+            self.service_id = m.get('service_id')
+        return self
+
+
+class QueryCaasContractServiceResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        data: ContractCreateProcessResp = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 请求结果数据
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('data') is not None:
+            temp_model = ContractCreateProcessResp()
+            self.data = temp_model.from_map(m['data'])
+        return self
+
+
+class PagequeryCaasContractMarketRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class PagequeryCaasContractMarketResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        version: str = None,
+        success: bool = None,
+        error_code: str = None,
+        error_msg: str = None,
+        data: List[ContractTemplateResp] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 响应版本号
+        self.version = version
+        # 请求是否成功
+        self.success = success
+        # 异常码
+        self.error_code = error_code
+        # 异常信息
+        self.error_msg = error_msg
+        # 请求结果数据
+        self.data = data
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.version is not None:
+            result['version'] = self.version
+        if self.success is not None:
+            result['success'] = self.success
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        result['data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['data'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('version') is not None:
+            self.version = m.get('version')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        self.data = []
+        if m.get('data') is not None:
+            for k in m.get('data'):
+                temp_model = ContractTemplateResp()
+                self.data.append(temp_model.from_map(k))
+        return self
+
+
 class CreateContractRecordRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         abi_oss_key: str = None,
         bizid: str = None,
@@ -56793,14 +59158,123 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('detail_url') is not None:
             self.detail_url = m.get('detail_url')
         return self
 
 
+class NotifyAuthTaskStatusRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        task_id: str = None,
+        user_id: str = None,
+        status: str = None,
+        happen_time: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 任务id
+        self.task_id = task_id
+        # 支uid
+        self.user_id = user_id
+        # NO_START, NO_SUBMIT, NOT_COMPLETE, COMPLETE
+        self.status = status
+        # 状态发生时间
+        self.happen_time = happen_time
+
+    def validate(self):
+        self.validate_required(self.task_id, 'task_id')
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.status, 'status')
+        self.validate_required(self.happen_time, 'happen_time')
+        if self.happen_time is not None:
+            self.validate_pattern(self.happen_time, 'happen_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.task_id is not None:
+            result['task_id'] = self.task_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.status is not None:
+            result['status'] = self.status
+        if self.happen_time is not None:
+            result['happen_time'] = self.happen_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('task_id') is not None:
+            self.task_id = m.get('task_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('happen_time') is not None:
+            self.happen_time = m.get('happen_time')
+        return self
+
+
+class NotifyAuthTaskStatusResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
 class StartDidCorporateAgentcreateRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         biz_code: str = None,
         extension_info: str = None,
```

### Comparing `antchain_blockchain-1.26.33/setup.py` & `antchain_blockchain-1.26.36/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_blockchain.
 
-Created on 09/02/2023
+Created on 26/07/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_blockchain"
 NAME = "antchain_blockchain" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BLOCKCHAIN SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

