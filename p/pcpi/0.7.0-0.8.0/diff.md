# Comparing `tmp/pcpi-0.7.0.tar.gz` & `tmp/pcpi-0.8.0.tar.gz`

## Comparing `pcpi-0.7.0.tar` & `pcpi-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pcpi-0.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pcpi-0.7.0/SUPPORT.md
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 pcpi-0.7.0/examples.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pcpi-0.7.0/min_requirements.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pcpi-0.7.0/requirements.txt
--rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 pcpi-0.7.0/run_tests.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pcpi-0.7.0/ssl_gen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcpi-0.7.0/src/pcpi/__init__.py
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pcpi-0.7.0/src/pcpi/_cspm_session.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 pcpi-0.7.0/src/pcpi/_onprem_cwp_session.py
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 pcpi-0.7.0/src/pcpi/_saas_cwp_session.py
--rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 pcpi-0.7.0/src/pcpi/_session_base.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pcpi-0.7.0/src/pcpi/_session_types.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 pcpi-0.7.0/src/pcpi/onprem_session_manager.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pcpi-0.7.0/src/pcpi/saas_session_manager.py
--rw-r--r--   0        0        0    37355 2020-02-02 00:00:00.000000 pcpi-0.7.0/src/pcpi/session_loader.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 pcpi-0.7.0/.gitignore
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pcpi-0.7.0/LICENSE
--rw-r--r--   0        0        0    18516 2020-02-02 00:00:00.000000 pcpi-0.7.0/README.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pcpi-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    20113 2020-02-02 00:00:00.000000 pcpi-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pcpi-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 pcpi-0.8.0/SUPPORT.md
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 pcpi-0.8.0/examples.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 pcpi-0.8.0/min_requirements.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pcpi-0.8.0/requirements.txt
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 pcpi-0.8.0/run_tests.py
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 pcpi-0.8.0/run_tests_old.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pcpi-0.8.0/ssl_gen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcpi-0.8.0/src/pcpi/__init__.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 pcpi-0.8.0/src/pcpi/_cspm_session.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 pcpi-0.8.0/src/pcpi/_onprem_cwp_session.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 pcpi-0.8.0/src/pcpi/_saas_cwp_session.py
+-rw-r--r--   0        0        0    23342 2020-02-02 00:00:00.000000 pcpi-0.8.0/src/pcpi/_session_base.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pcpi-0.8.0/src/pcpi/_session_types.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pcpi-0.8.0/src/pcpi/onprem_session_manager.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pcpi-0.8.0/src/pcpi/saas_session_manager.py
+-rw-r--r--   0        0        0    40286 2020-02-02 00:00:00.000000 pcpi-0.8.0/src/pcpi/session_loader.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 pcpi-0.8.0/.gitignore
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 pcpi-0.8.0/LICENSE
+-rw-r--r--   0        0        0    18386 2020-02-02 00:00:00.000000 pcpi-0.8.0/README.md
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pcpi-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    19983 2020-02-02 00:00:00.000000 pcpi-0.8.0/PKG-INFO
```

### Comparing `pcpi-0.7.0/CONTRIBUTING.md` & `pcpi-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pcpi-0.7.0/SUPPORT.md` & `pcpi-0.8.0/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `pcpi-0.7.0/examples.py` & `pcpi-0.8.0/examples.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.7.0/run_tests.py` & `pcpi-0.8.0/run_tests_old.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import unittest
 from unittest import mock
 from unittest import TestCase
 import os
-import yaml
+import json
 
 #Default Logger
 import logging
 logging.basicConfig()
 py_logger = logging.getLogger("pcpi")
 py_logger.setLevel(10)
 
 #HELPER FUNCTIONS==============================================================
 def load_environment():
     cfg = {}
-    with open('tenant_credentials.yml', "r") as file:
-        cfg = yaml.load(file, Loader=yaml.BaseLoader)
+    with open('local.json', "r") as file:
+        cfg = json.load(file)
 
     #Parse cfg for tenant creds and set env
-    for index,tenant in enumerate(cfg):
-        uname = cfg[tenant]['access_key']
-        passwd = cfg[tenant]['secret_key']
-        api_url = cfg[tenant]['api_url']
+    for index,cred in enumerate(cfg):
+        tenant = cred['name']
+        uname = cred['access_key']
+        passwd = cred['secret_key']
+        api_url = cred['api_url']
         verify = True
         try:
-            verify = cfg[tenant]['verify']
+            verify = cred['verify']
             if verify.lower() == 'false':
                 verify = False
             if verify.lower() == 'true':
                 verify = True
         except:
             pass
         
         os.environ[f'PC_TENANT_NAME{index}'] = tenant
         os.environ[f'PC_TENANT_API{index}'] = api_url
         os.environ[f'PC_TENANT_A_KEY{index}'] = uname
         os.environ[f'PC_TENANT_S_KEY{index}'] = passwd
         os.environ[f'PC_TENANT_VERIFY{index}'] = str(verify)
+        os.environ[f'PC_HTTP_PROXY{index}'] = cred['http_proxy']
+        os.environ[f'PC_HTTPS_PROXY{index}'] = cred['https_proxy']
 
 def load_onprem_environment():
     cfg = {}
     with open('console_credentials.yml', "r") as file:
         cfg = yaml.load(file, Loader=yaml.BaseLoader)
 
     #Parse cfg for tenant names and create tokens for each tenant
```

### Comparing `pcpi-0.7.0/ssl_gen.py` & `pcpi-0.8.0/ssl_gen.py`

 * *Files identical despite different names*

### Comparing `pcpi-0.7.0/src/pcpi/_cspm_session.py` & `pcpi-0.8.0/src/pcpi/_cspm_session.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #Local
 from ._session_base import Session
 
 import time
 
 #++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class CSPMSession(Session):
-    def __init__(self, tenant_name: str, a_key: str, s_key: str, api_url: str, verify, logger):
+    def __init__(self, tenant_name: str, a_key: str, s_key: str, api_url: str, verify: bool, proxies: dict, logger):
         """
         Initializes a Prisma Cloud API session for a given tenant.
 
         Keyword arguments:
         tenant_name -- Name of tenant associated with session
         a_key -- Tenant Access Key
         s_key -- Tenant Secret Key
@@ -24,14 +24,15 @@
         super().__init__(logger)
 
         self.tenant = tenant_name
         self.a_key = a_key
         self.s_key = s_key
         self.api_url = api_url
         self.verify = verify
+        self.proxies = proxies
 
         self.token_time_stamp = 0
 
         self.token = ''
 
         self.auth_key = 'x-redlock-auth'
         self.auth_style = ''
@@ -64,15 +65,15 @@
         }
 
         self.logger.debug('API - Generating CSPM session token.')
         res = object()
         try:
             start_time = time.time()
             self.logger.debug(url)
-            res = requests.request("POST", url, headers=headers, json=payload, verify=self.verify)
+            res = requests.request("POST", url, headers=headers, json=payload, verify=self.verify, proxies=self.proxies)
             end_time = time.time()
             time_completed = round(end_time-start_time,3)
 
             self.token_time_stamp = time.time()
         except:
             self.logger.error('Failed to connect to API.')
             self.logger.warning('Make sure any offending VPNs are disabled.')
@@ -87,15 +88,15 @@
     def _api_refresh(self) -> None:
             self.logger.debug('API - Refreshing SaaS session token.')
 
             res = object()
             try:
                 start_time = time.time()
                 self.logger.debug(self.api_url + '/auth_token/extend')
-                res = requests.request("GET", self.api_url + '/auth_token/extend', headers=self.headers, verify=self.verify)
+                res = requests.request("GET", self.api_url + '/auth_token/extend', headers=self.headers, verify=self.verify, proxies=self.proxies)
                 end_time = time.time()
                 time_completed = round(end_time-start_time,3)
                 self.token_time_stamp = time.time()
             except:
                 self.logger.error('Failed to connect to API.')
                 self.logger.warning('Make sure any offending VPNs are disabled.')
```

### Comparing `pcpi-0.7.0/src/pcpi/_onprem_cwp_session.py` & `pcpi-0.8.0/src/pcpi/_onprem_cwp_session.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #Local
 from ._session_base import Session
 
 import time
 
 #++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class CWPSession(Session):
-    def __init__(self, tenant_name: str, api_url: str, uname: str, passwd:str, verify:bool, project_flag:bool, logger: object):
+    def __init__(self, tenant_name: str, api_url: str, uname: str, passwd:str, verify:bool, proxies: dict, project_flag:bool, logger: object):
         """
         Initializes a Prisma Cloud API session for a given tenant.
 
         Keyword Arguments:
         tenant_name -- Name of tenant associated with session
         api_url -- API URL Tenant is hosted on
         uname -- Username
@@ -28,14 +28,15 @@
 
         super().__init__(logger)
 
         self.tenant = tenant_name
         self.uname = uname
         self.passwd = passwd
         self.verify = verify
+        self.proxies = proxies
         self.project_flag = project_flag
 
         self.token_time_stamp = 0
 
         self.api_url = api_url
 
         self.logger = logger
@@ -73,15 +74,15 @@
 
         self.logger.debug('API - Generating CWP session token.')
 
         res = object()
         try:
             start_time = time.time()
             self.logger.debug(url)
-            res = requests.request("POST", url, headers=headers, json=payload, verify=self.verify)
+            res = requests.request("POST", url, headers=headers, json=payload, verify=self.verify, proxies=self.proxies)
             end_time = time.time()
             time_completed = round(end_time-start_time, 3)
 
             self.token_time_stamp = time.time()
         except:
             self.logger.error('Failed to connect to API.')
             self.logger.warning('Make sure any offending VPNs are disabled.')
```

### Comparing `pcpi-0.7.0/src/pcpi/_saas_cwp_session.py` & `pcpi-0.8.0/src/pcpi/_saas_cwp_session.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ._cspm_session import CSPMSession
 
 #Python Library
 import time
 
 #++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 class SaaSCWPSession(Session):
-    def __init__(self, tenant_name: str, a_key: str, s_key: str, api_url: str, verify, logger, cspm_session={}):
+    def __init__(self, tenant_name: str, a_key: str, s_key: str, api_url: str, verify: bool, proxies: dict, logger, cspm_session={}):
         """
         Initializes a Prisma Cloud API session for a given tenant.
 
         Keyword Arguments:
         tenant_name -- Name of tenant associated with session
         a_key -- Tenant Access Key
         s_key -- Tenant Secret Key
@@ -27,14 +27,15 @@
         super().__init__(logger)
 
         self.tenant = tenant_name
         self.a_key = a_key
         self.s_key = s_key
         self.api_url = api_url
         self.verify = verify
+        self.proxies = proxies
 
         self.token_time_stamp = 0
 
         self.logger = logger
 
         self.cspm_session = {}
         self.cspm_token = ''
@@ -57,15 +58,15 @@
             'Authorization': 'Bearer '
         }
 
         self._api_login_wrapper()
 
 #==============================================================================
     def __get_cspm_session(self):
-        self.cspm_session = CSPMSession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, self.logger)
+        self.cspm_session = CSPMSession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, self.proxies, self.logger)
         self.cspm_token = self.cspm_session.token
     
     def __cspm_login(self):
         self.cspm_token = self.cspm_session._api_login_wrapper()
 
     def __cwpp_metadata(self, cspm_session):
         res = cspm_session.request('GET', 'meta_info')
@@ -97,15 +98,15 @@
 
         self.logger.debug('API - Generating SaaS CWPP session token.')
 
         res = object()
         try:
             start_time = time.time()
             self.logger.debug(url)
-            res = requests.request("POST", url, headers=headers, json=payload, verify=self.verify)
+            res = requests.request("POST", url, headers=headers, json=payload, verify=self.verify, proxies=self.proxies)
             end_time = time.time()
             time_completed = round(end_time-start_time, 3)
             
             self.token_time_stamp = time.time()
         except:
             self.logger.error('Failed to connect to API.')
             self.logger.warning('Make sure any offending VPNs are disabled.')
```

### Comparing `pcpi-0.7.0/src/pcpi/_session_base.py` & `pcpi-0.8.0/src/pcpi/_session_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                     self.logger.warning('Steps to troubleshoot: ')
                     self.logger.warning('1) Disable any VPNs.')
                     self.logger.warning('2) Ensure API base URL is correct.')
                     time.sleep(1)
 
 
 #==============================================================================
-    def __api_call_wrapper(self, method: str, url: str, json: dict=None, data: dict=None, params: dict=None, verify=True, acceptCsv=False, redlock_ignore: list=None, status_ignore: list=[], custom_log='', custom_error_message=''):
+    def __api_call_wrapper(self, method: str, url: str, json: dict=None, data: dict=None, params: dict=None, verify=True, proxies=None, acceptCsv=False, redlock_ignore: list=None, status_ignore: list=[], custom_log='', custom_error_message=''):
         """
         A wrapper around all API calls that handles token generation, retrying
         requests and API error console output logging.
         Keyword Arguments:
         method -- Request method/type. Ex: POST or GET
         url -- Full API request URL
         data -- Body of the request in a json compatible format
@@ -224,15 +224,15 @@
         while res == self.empty_res and self.u_count < self.unknown_error_max:
             try:
                 if time.time() - self.token_time_stamp >= self.token_time:
                     self.logger.warning('Session Refresh Timer - Generating new Token')
                     self._api_refresh_wrapper()
 
                 self.logger.debug(f'{url}')
-                res,time_completed = self.__request_wrapper(method, url, headers=self.headers, json=json, data=data, params=params, verify=verify, acceptCsv=acceptCsv)
+                res,time_completed = self.__request_wrapper(method, url, headers=self.headers, json=json, data=data, params=params, verify=verify, proxies=proxies, acceptCsv=acceptCsv)
                 
                 if res.status_code in self.success_status or res.status_code in status_ignore:
                     log_message = ''
                     if custom_log:
                         log_message = ' - ' + custom_log
 
                     try:
@@ -282,15 +282,15 @@
                         self.logger.warning('Session expired. Generating new Token and retrying')
                         self._api_login_wrapper()
                         encountered_401 = True
 
                     self.logger.warning(f'Retrying request')
                     self.logger.debug(f'{url}')
 
-                    res, time_completed = self.__request_wrapper(method, url, headers=self.headers, json=json, data=data, params=params, verify=verify, acceptCsv=acceptCsv)
+                    res, time_completed = self.__request_wrapper(method, url, headers=self.headers, json=json, data=data, params=params, verify=verify, proxies=proxies, acceptCsv=acceptCsv)
                     retries += 1
                 
                 if res.status_code in self.success_status or res.status_code in status_ignore:
                     try:
                         self.logger.success(f'SUCCESS - {time_completed} seconds')
                     except:
                         self.logger.info(f'SUCCESS - {time_completed} seconds')
@@ -352,23 +352,26 @@
                     time.sleep(2)
                 else:
                     self.logger.error(f'UNKNOWN ERROR - API Call Wrapper. Continuing... {self.u_count} of {self.unknown_error_max}')
                 self.u_count += 1
 
     #==============================================================================
 
-    def request(self, method: str, endpoint_url: str, json: dict=None, data: dict=None, params: dict=None, verify=None, acceptCsv=False, redlock_ignore: list=None, status_ignore: list=[], custom_log='', custom_error_message=''):
+    def request(self, method: str, endpoint_url: str, json: dict=None, data: dict=None, params: dict=None, verify=None, proxies=None, acceptCsv=False, redlock_ignore: list=None, status_ignore: list=[], custom_log='', custom_error_message=''):
         '''
         Function for calling the PC API using this session manager. Accepts the
         same arguments as 'requests.request' minus the headers argument as 
         headers are supplied by the session manager.
         '''
         if verify == None:
             verify = self.verify
 
+        if proxies == None:
+            proxies = self.proxies
+
         #If the CWP Session is a project, auto add project id query string
         try:
             if self.project_flag == True:
                 if params:
                     params.update({"project":self.tenant})
                 else:
                     params = {"project":self.tenant}
@@ -383,27 +386,31 @@
         #Build url
         if endpoint_url[0] != '/':
             endpoint_url = '/' + endpoint_url
 
         url = f'{self.api_url}{endpoint_url}'
 
         #Call wrapper
-        return self.__api_call_wrapper(method, url, json=json, data=data, params=params, verify=verify, acceptCsv=acceptCsv, redlock_ignore=redlock_ignore, status_ignore=status_ignore, custom_log=custom_log, custom_error_message=custom_error_message)
+        return self.__api_call_wrapper(method, url, json=json, data=data, params=params, verify=verify, proxies=proxies, acceptCsv=acceptCsv, redlock_ignore=redlock_ignore, status_ignore=status_ignore, custom_log=custom_log, custom_error_message=custom_error_message)
 
-    def config_search_request(self, json: dict, verify=None, redlock_ignore: list=None, status_ignore: list=[]):
+    def config_search_request(self, json: dict, verify=None, proxies=None, redlock_ignore: list=None, status_ignore: list=[]):
         if verify == None:
             verify = self.verify
+
+        if proxies == None:
+            proxies = self.proxies
+
         
         limit = 2000#Max limit value is 100,000
         
         #Force best practices with HS
         json.update({"heuristicSearch": True, "limit": limit, "withResourceJson": True})
 
         #initial API Call
-        res = self.__api_call_wrapper('POST', f'{self.api_url}/search/config', json=json, verify=verify, redlock_ignore=redlock_ignore, status_ignore=status_ignore)
+        res = self.__api_call_wrapper('POST', f'{self.api_url}/search/config', json=json, verify=verify, proxies=proxies, redlock_ignore=redlock_ignore, status_ignore=status_ignore)
 
         total_rows = 0
         complete_res_list = []
         complete_res_dict = res.json()
 
         #res_data var used for while loop
         res_data = res.json()['data']
@@ -415,15 +422,15 @@
 
         counter = 0
         while 'nextPageToken' in res_data:
             #update payload
             json.update({'pageToken': res_data.get('nextPageToken')})
 
             #call page endpoint
-            res = self.__api_call_wrapper('POST', f'{self.api_url}/search/config/page', json=json, verify=verify, redlock_ignore=redlock_ignore, status_ignore=status_ignore)
+            res = self.__api_call_wrapper('POST', f'{self.api_url}/search/config/page', json=json, verify=verify, proxies=proxies, redlock_ignore=redlock_ignore, status_ignore=status_ignore)
             counter += 1
 
             #update res_data with the paginated response
             res_data = res.json()
 
             #Add results from each page API call
             complete_res_list.extend(res_data.get('items'))
@@ -432,25 +439,29 @@
             total_rows+= retrievedRows
 
         #Update res dict to be the some format as the 'data' object in a typical RQL res
         complete_res_dict['data'].update({'totalRows':total_rows, 'items': complete_res_list})
 
         return complete_res_dict
 
-    def config_search_request_function(self, json, function, verify=None, redlock_ignore: list=None, status_ignore: list=[]):
+    def config_search_request_function(self, json, function, verify=None, proxies=None, redlock_ignore: list=None, status_ignore: list=[]):
         if verify == None:
             verify = self.verify
+
+        if proxies == None:
+            proxies = self.proxies
+
         
         limit = 2000#Max limit value is 100,000
         
         #Force best practices with HS
         json.update({"heuristicSearch": True, "limit": limit, "withResourceJson": True})
 
         #initial API Call
-        res = self.__api_call_wrapper('POST', f'{self.api_url}/search/config', json=json, verify=verify, redlock_ignore=redlock_ignore, status_ignore=status_ignore)
+        res = self.__api_call_wrapper('POST', f'{self.api_url}/search/config', json=json, verify=verify, proxies=proxies, redlock_ignore=redlock_ignore, status_ignore=status_ignore)
         
         total_rows = res.json()['data']['totalRows']
 
         res_details = res.json()
         res_details.pop('data')
         res_data = res.json()['data']
         counter = 0
@@ -458,41 +469,41 @@
         function(res_details, res_data, counter, total_rows)
 
         while 'nextPageToken' in res_data:
             #update payload
             json.update({'pageToken': res_data.get('nextPageToken')})
 
             #call page endpoint
-            res = self.__api_call_wrapper('POST', f'{self.api_url}/search/config/page', json=json, verify=verify, redlock_ignore=redlock_ignore, status_ignore=status_ignore)
+            res = self.__api_call_wrapper('POST', f'{self.api_url}/search/config/page', json=json, verify=verify, proxies=proxies, redlock_ignore=redlock_ignore, status_ignore=status_ignore)
             counter += 1
 
             res_data = res.json()
             total_rows += res_data['totalRows']
 
             function(res_details, res_data, counter, total_rows)
 
         return total_rows
 
-    def __request_wrapper(self, method, url, headers, json, data, params, verify, acceptCsv):
+    def __request_wrapper(self, method, url, headers, json, data, params, verify, proxies, acceptCsv):
         if acceptCsv == True: #CSPM Support Only
             headers.update({
                 'Accept': 'text/csv'
             })
 
         r = self.empty_res
 
         start_time = time.time()
-        r = requests.request(method, url, headers=headers, json=json, data=data, params=params, verify=verify)
+        r = requests.request(method, url, headers=headers, json=json, data=data, params=params, verify=verify, proxies=proxies)
         end_time = time.time()
         time_completed = round(end_time-start_time,3)
 
         while r == self.empty_res and self.u_count < self.unknown_error_max:
             try:
                 start_time = time.time()
-                r = requests.request(method, url, headers=headers, json=json, data=data, params=params, verify=verify)
+                r = requests.request(method, url, headers=headers, json=json, data=data, params=params, verify=verify, proxies=proxies)
                 end_time = time.time()
                 time_completed = round(end_time-start_time,3)
 
                 self.u_count = 1
                 return [r, time_completed]
             except KeyboardInterrupt:
                 self.logger.error('Keyboard Interrupt. Exiting...')
```

### Comparing `pcpi-0.7.0/src/pcpi/onprem_session_manager.py` & `pcpi-0.8.0/src/pcpi/onprem_session_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 
 logging.basicConfig()
 py_logger = logging.getLogger("pcpi")
 py_logger.setLevel(10)
 
 class CWPSessionManager:
-    def __init__(self, tenant_name: str, api_url: str, uname: str, passwd: str, verify:bool=True, project_flag:bool=False, logger:object=py_logger):
+    def __init__(self, tenant_name: str, api_url: str, uname: str, passwd: str, verify:bool=True, proxies:dict=None, project_flag:bool=False, logger:object=py_logger):
         """
         Initializes a Prisma Cloud API Session Manager.
 
         Keyword Arguments:
         tenant_name -- Name of tenant associated with session
         a_key -- Tenant Access Key
         s_key -- Tenant Secret Key
@@ -21,17 +21,18 @@
     
         self.tenant = tenant_name
         self.uname = uname
         self.passwd = passwd
         self.api_url = api_url
 
         self.verify = verify
+        self.proxies = proxies
         self.project_flag = project_flag
 
         self.cwp_session = {}        
 
 
 #==============================================================================
     def create_cwp_session(self):
-        session = CWPSession(self.tenant, self.api_url, self.uname, self.passwd, self.verify, self.project_flag, self.logger)
+        session = CWPSession(self.tenant, self.api_url, self.uname, self.passwd, self.verify, self.proxies, self.project_flag, self.logger)
         self.cwp_session = session
         return session
```

### Comparing `pcpi-0.7.0/src/pcpi/saas_session_manager.py` & `pcpi-0.8.0/src/pcpi/saas_session_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 py_logger = logging.getLogger("pcpi")
 py_logger.setLevel(10)
 
 #Local
 from ._session_types import CSPMSession, SaaSCWPSession
 
 class SaaSSessionManager:
-    def __init__(self, tenant_name: str, a_key: str, s_key: str, api_url: str, verify=True, logger=py_logger):
+    def __init__(self, tenant_name: str, a_key: str, s_key: str, api_url: str, verify=True, proxies:dict=None, logger=py_logger):
         """
         Initializes a Prisma Cloud API Session Manager.
 
         Keyword Arguments:
         tenant_name -- Name of tenant associated with session
         a_key -- Tenant Access Key
         s_key -- Tenant Secret Key
@@ -24,32 +24,33 @@
 
         self.tenant = tenant_name
         self.a_key = a_key
         self.s_key = s_key
         self.api_url = api_url
 
         self.verify = verify
+        self.proxies = proxies
 
         self.cspm_session = {}
         self.saas_cwp_session = {}
         
 
 
 #==============================================================================
     def create_cspm_session(self):
-        session = CSPMSession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, logger=self.logger)
+        session = CSPMSession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, self.proxies, logger=self.logger)
         self.cspm_session = session
         return session
     
     def create_cwp_session(self):
         if self.cspm_session:
-            session = SaaSCWPSession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, logger=self.logger, cspm_session=self.cspm_session)
+            session = SaaSCWPSession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, self.proxies, logger=self.logger, cspm_session=self.cspm_session)
             self.saas_cwp_session = session
             return session
         else:
             self.create_cspm_session()
-            session = SaaSCWPSession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, logger=self.logger, cspm_session=self.cspm_session)
+            session = SaaSCWPSession(self.tenant, self.a_key, self.s_key, self.api_url, self.verify, self.proxies, logger=self.logger, cspm_session=self.cspm_session)
             self.saas_cwp_session = session
             return session
 
 
 #==============================================================================
```

### Comparing `pcpi-0.7.0/src/pcpi/session_loader.py` & `pcpi-0.8.0/src/pcpi/session_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     print(f'{color}', end='')
     for val in args:
         print(val, end='')
     print(f'{c_end}', end=_end)
 
 #==============================================================================
 
-def __validate_cwp_credentials(name, _url, uname, passwd, verify) -> bool:
+def __validate_cwp_credentials(name, _url, uname, passwd, verify, proxies) -> bool:
     '''
     This function creates a session with the supplied credentials to test 
     if the user successfully entered valid credentials.
     '''
 
     headers = {
     'content-type': 'application/json; charset=UTF-8'
@@ -79,15 +79,15 @@
         "password": passwd,
     }
 
     url = f'{_url}/api/v1/authenticate'
 
     try:
         __c_print('API - Validating credentials')
-        res = requests.request("POST", url, headers=headers, json=payload, verify=verify)
+        res = requests.request("POST", url, headers=headers, json=payload, verify=verify, proxies=proxies)
         print(res.status_code)
 
         if res.status_code == 200:
             __c_print('SUCCESS', color='green')
             print()
             return True
         else:
@@ -99,15 +99,15 @@
         print('Steps to troubleshoot:')
         __c_print('1) Please disconnect from any incompatible VPN', color='blue')
         print()
         __c_print('2) Please ensure you have entered a valid Prisma Cloud URL.', color='blue')
         print()
         return False
 
-def __validate_credentials(a_key, s_key, url, verify) -> bool:
+def __validate_credentials(a_key, s_key, url, verify, proxies) -> bool:
     '''
     This function creates a session with the supplied credentials to test 
     if the user successfully entered valid credentials.
     '''
 
     headers = {
     'content-type': 'application/json; charset=UTF-8'
@@ -116,15 +116,15 @@
     payload = {
         "username": f"{a_key}",
         "password": f"{s_key}"
     }
 
     try:
         __c_print('API - Validating credentials')
-        response = requests.request("POST", f'{url}/login', headers=headers, json=payload, verify=verify)
+        response = requests.request("POST", f'{url}/login', headers=headers, json=payload, verify=verify, proxies=proxies)
 
         if response.status_code == 200:
             __c_print('SUCCESS', color='green')
             print()
             return True
         else:
             return False
@@ -136,23 +136,23 @@
         __c_print('1) Please disconnect from any incompatible VPN', color='blue')
         print()
         __c_print('2) Please ensure you have entered a valid Prisma Cloud URL.', color='blue')
         print('EX: https://app.prismacloud.io or https://app2.eu.prismacloud.io')
         print()
         return False
 
-def __universal_validate_credentials(name, url, _id, secret, verify):
+def __universal_validate_credentials(name, url, _id, secret, verify, proxies):
     if verify.lower() == 'true':
         verify = True
     else:
         verify = False
     if 'prismacloud.io' in url or 'prismacloud.cn' in url:
-        return __validate_credentials(_id, secret, url, verify)
+        return __validate_credentials(_id, secret, url, verify, proxies)
     else:
-        return __validate_cwp_credentials(name, url, _id, secret, verify)
+        return __validate_cwp_credentials(name, url, _id, secret, verify, proxies)
 
 #==============================================================================
 
 def __validate_url(url):
     if "prismacloud.io" not in (url):
         if 'https://' not in url and 'http://' not in url:
             url = 'https://' + url
@@ -189,24 +189,43 @@
     print()
 
     __c_print('Certificate verification: (True/False/<path to .pem file>)', color='blue')
     __c_print('Leave blank to use default value.', color='yellow')
     verify = input()
     print()
 
+    __c_print('Proxy section. HTTP first, HTTPS second. Leave blank to not use a proxy.', color='blue')
+
+    __c_print('Enter HTTP proxy address.', color='blue')
+    __c_print('If you are not using a proxy, leave blank.', color='yellow')
+    http_proxy = input()
+    print()
+
+    __c_print('Enter HTTPS proxy address.', color='blue')
+    __c_print('If you are not using a proxy, leave blank.', color='yellow')
+    https_proxy = input()
+    print()
+    
+    proxies = None
+    if http_proxy or https_proxy:
+        proxies = {
+            'http': http_proxy,
+            'https': https_proxy
+        }
+
     if verify == '':
         verify = True
     elif verify.lower() == 'true':
         verify = True
     elif verify.lower() == 'false':
         verify = False
     else:
         pass
 
-    return name, url, uname, passwd, verify
+    return name, url, uname, passwd, verify, proxies
 
 def __get_config():
     __c_print('Enter Prisma URL. (SaaS EX: https://app.ca.prismacloud.io, On-Prem EX: https://yourdomain.com):', color='blue')
     url = input()
     print()
     new_url = __validate_url(url)
     if new_url != url:
@@ -223,14 +242,33 @@
     print()
 
     __c_print('Certificate verification: (True/False/<path_to_.pem> file)', color='blue')
     __c_print('Leave blank to use default value (True).', color='yellow')
     verify = input()
     print()
 
+    __c_print('Proxy section. HTTP first, HTTPS second. Leave blank to not use a proxy.', color='yellow')
+
+    __c_print('Enter HTTP proxy address.', color='blue')
+    __c_print('If you are not using a proxy, leave blank.', color='yellow')
+    http_proxy = input()
+    print()
+
+    __c_print('Enter HTTPS proxy address.', color='blue')
+    __c_print('If you are not using a proxy, leave blank.', color='yellow')
+    https_proxy = input()
+    print()
+    
+    proxies = None
+    if http_proxy or https_proxy:
+        proxies = {
+            'http': http_proxy,
+            'https': https_proxy
+        }
+
     #If there is non-prisma URL, then ask if its a self hosted project
     project_flag = 'false'
     if 'prismacloud.io' not in new_url and 'prismacloud.cn' not in new_url:
         __c_print('CWP Project (True/False)', color='blue')
         __c_print('Leave blank to use default value (False).', color='yellow')
         project_flag = input()
         print()
@@ -257,15 +295,15 @@
         verify = 'true'
     elif verify.lower() == 'false':
         verify = 'false'
     else:
         pass
     
 
-    return name, _id, secret, new_url, verify, project_flag
+    return name, _id, secret, new_url, verify, proxies, project_flag
 
 def __get_tenant_credentials():
 
     __c_print('Enter tenant name or any preferred identifier (optional):', color='blue')
     name = input()
 
     __c_print('Enter tenant url. (ex: https://app.ca.prismacloud.io):', color='blue')
@@ -286,57 +324,79 @@
     print()
 
     __c_print('Certificate verification: (True/False/<path to .pem file>)', color='blue')
     __c_print('Leave blank to use default value.', color='yellow')
     verify = input()
     print()
 
+    __c_print('Proxy section. HTTP first, HTTPS second. Leave blank to not use a proxy.', color='blue')
+
+    __c_print('Enter HTTP proxy address.', color='blue')
+    __c_print('If you are not using a proxy, leave blank.', color='yellow')
+    http_proxy = input()
+    print()
+
+    __c_print('Enter HTTPS proxy address.', color='blue')
+    __c_print('If you are not using a proxy, leave blank.', color='yellow')
+    https_proxy = input()
+    print()
+    
+    proxies = None
+    if http_proxy or https_proxy:
+        proxies = {
+            'http': http_proxy,
+            'https': https_proxy
+        }
+
     if verify == '':
         verify = True
     elif verify.lower() == 'true':
         verify = True
     elif verify.lower() == 'false':
         verify = False
     else:
         pass
     
 
-    return name, a_key, s_key, new_url, verify
+    return name, a_key, s_key, new_url, verify, proxies
 
 #==============================================================================
 
-def __build_cwp_session_dict(name, url, uname, passwd, verify):
+def __build_cwp_session_dict(name, url, uname, passwd, verify, proxies):
     session_dict = {
         name: {
             'url': url,
             'uname': uname,
             'passwd': passwd,
-            'verify': verify
+            'verify': verify,
+            'proxies': proxies
             }
     }
     return session_dict
 
-def __build_session_dict(name, a_key, s_key, url, verify):
+def __build_session_dict(name, a_key, s_key, url, verify, proxies):
     session_dict = {
         name: {
             'access_key': a_key,
             'secret_key': s_key,
             'api_url': url,
-            'verify': verify
+            'verify': verify,
+            'proxies': proxies
             }
     }
     return session_dict
 
-def __build_config_json(name, _id, secret, url, verify, project_flag):
+def __build_config_json(name, _id, secret, url, verify, proxies, project_flag):
     session_dict = {
         'name': name,
         'url': url,
         'identity': _id,
         'secret': secret,
         'verify': verify,
+        'proxies': proxies,
         'project_flag': project_flag
     }
     return session_dict
 
 #==============================================================================
 
 def __get_min_cwp_credentials_from_user(min_tenants):
@@ -344,23 +404,23 @@
     tenants_added = 0
 
     while True:
         valid = False
         while not valid:
             __c_print('Enter credentials for the console', color='blue')
             print()
-            name, url, uname, passwd, verify = __get_cwp_tenant_credentials()
+            name, url, uname, passwd, verify, proxies = __get_cwp_tenant_credentials()
             
-            valid = __validate_cwp_credentials(name, url, uname, passwd, verify)
+            valid = __validate_cwp_credentials(name, url, uname, passwd, verify, proxies)
             if valid == False:
                 __c_print('FAILED', end=' ', color='red')
                 print('Invalid credentials. Please re-enter your credentials')
                 print()
             else:
-                credentials.append(__build_cwp_session_dict(name, url, uname, passwd, verify))
+                credentials.append(__build_cwp_session_dict(name, url, uname, passwd, verify, proxies))
                 tenants_added += 1
         
         if tenants_added >= min_tenants:
             __c_print('Would you like to add an other tenant? Y/N')
             choice = input().lower()
 
             if choice != 'yes' and choice != 'y':
@@ -374,40 +434,40 @@
 
     if num_tenants != -1:
         for i in range(num_tenants):
             valid = False
             while not valid:
                 __c_print('Enter credentials for the console', color='blue')
                 print()
-                name, url, uname, passwd, verify = __get_cwp_tenant_credentials()
+                name, url, uname, passwd, verify, proxies = __get_cwp_tenant_credentials()
                 
-                valid = __validate_cwp_credentials(name, url, uname, passwd, verify)
+                valid = __validate_cwp_credentials(name, url, uname, passwd, verify, proxies)
                 if valid == False:
                     __c_print('FAILED', end=' ', color='red')
                     print('Invalid credentials. Please re-enter your credentials')
                     print()
                 else:
-                    credentials.append(__build_cwp_session_dict(name, url, uname, passwd, verify))
+                    credentials.append(__build_cwp_session_dict(name, url, uname, passwd, verify, proxies))
 
         return credentials
     else:
         while True:
             valid = False
             while not valid:
                 __c_print('Enter credentials for the console', color='blue')
                 print()
-                name, url, uname, passwd, verify = __get_cwp_tenant_credentials()
+                name, url, uname, passwd, verify, proxies = __get_cwp_tenant_credentials()
                 
-                valid = __validate_cwp_credentials(name, url, uname, passwd, verify)
+                valid = __validate_cwp_credentials(name, url, uname, passwd, verify, proxies)
                 if valid == False:
                     __c_print('FAILED', end=' ', color='red')
                     print('Invalid credentials. Please re-enter your credentials')
                     print()
                 else:
-                    credentials.append(__build_cwp_session_dict(name, url, uname, passwd, verify))
+                    credentials.append(__build_cwp_session_dict(name, url, uname, passwd, verify, proxies))
             
             __c_print('Would you like to add an other tenant? Y/N')
             choice = input().lower()
 
             if choice != 'yes' and choice != 'y':
                 break
 
@@ -417,23 +477,23 @@
     credentials = []
     tenants_added = 0
     while True:
         valid = False
         while not valid:
             __c_print('Enter credentials for the tenant', color='blue')
             print()
-            src_name, src_a_key, src_s_key, src_url, verify = __get_tenant_credentials()
+            src_name, src_a_key, src_s_key, src_url, verify, proxies = __get_tenant_credentials()
             
-            valid = __validate_credentials(src_a_key, src_s_key, src_url, verify)
+            valid = __validate_credentials(src_a_key, src_s_key, src_url, verify, proxies)
             if valid == False:
                 __c_print('FAILED', end=' ', color='red')
                 print('Invalid credentials. Please re-enter your credentials')
                 print()
             else:
-                credentials.append(__build_session_dict(src_name, src_a_key, src_s_key, src_url, verify))
+                credentials.append(__build_session_dict(src_name, src_a_key, src_s_key, src_url, verify, proxies))
                 tenants_added += 1
         
         if tenants_added >= min_tenants:
             __c_print('Would you like to add an other tenant? Y/N')
             choice = input().lower()
 
             if choice != 'yes' and choice != 'y':
@@ -447,40 +507,40 @@
 
     if num_tenants != -1:
         for i in range(num_tenants):
             valid = False
             while not valid:
                 __c_print('Enter credentials for the tenant', color='blue')
                 print()
-                src_name, src_a_key, src_s_key, src_url, verify = __get_tenant_credentials()
+                src_name, src_a_key, src_s_key, src_url, verify, proxies = __get_tenant_credentials()
                 
-                valid = __validate_credentials(src_a_key, src_s_key, src_url, verify)
+                valid = __validate_credentials(src_a_key, src_s_key, src_url, verify, proxies)
                 if valid == False:
                     __c_print('FAILED', end=' ', color='red')
                     print('Invalid credentials. Please re-enter your credentials')
                     print()
                 else:
-                    credentials.append(__build_session_dict(src_name, src_a_key, src_s_key, src_url, verify))
+                    credentials.append(__build_session_dict(src_name, src_a_key, src_s_key, src_url, verify, proxies))
 
         return credentials
     else:
         while True:
             valid = False
             while not valid:
                 __c_print('Enter credentials for the tenant', color='blue')
                 print()
-                src_name, src_a_key, src_s_key, src_url, verify = __get_tenant_credentials()
+                src_name, src_a_key, src_s_key, src_url, verify, proxies = __get_tenant_credentials()
                 
-                valid = __validate_credentials(src_a_key, src_s_key, src_url, verify)
+                valid = __validate_credentials(src_a_key, src_s_key, src_url, verify, proxies)
                 if valid == False:
                     __c_print('FAILED', end=' ', color='red')
                     print('Invalid credentials. Please re-enter your credentials')
                     print()
                 else:
-                    credentials.append(__build_session_dict(src_name, src_a_key, src_s_key, src_url, verify))
+                    credentials.append(__build_session_dict(src_name, src_a_key, src_s_key, src_url, verify, proxies))
             
             __c_print('Would you like to add an other tenant? Y/N')
             choice = input().lower()
 
             if choice != 'yes' and choice != 'y':
                 break
 
@@ -492,61 +552,61 @@
 
     if num_tenants != -1 and min_tenants == -1:
         for i in range(num_tenants):
             valid = False
             while not valid:
                 __c_print('Enter Prisma Cloud Credentials', color='blue')
                 print()
-                name, _id, secret, url, verify, project_flag = __get_config()
+                name, _id, secret, url, verify, proxies, project_flag = __get_config()
                 
-                valid = __universal_validate_credentials(name, url, _id, secret, verify)
+                valid = __universal_validate_credentials(name, url, _id, secret, verify, proxies)
                 if valid == False:
                     __c_print('FAILED', end=' ', color='red')
                     print('Invalid credentials. Please re-enter your credentials')
                     print()
                 else:
-                    credentials.append(__build_config_json(name, _id, secret, url, verify, project_flag))
+                    credentials.append(__build_config_json(name, _id, secret, url, verify, proxies, project_flag))
     elif num_tenants == -1 and min_tenants != -1:
         tenant_count = 0
         while True:
             valid = False
             while not valid:
                 __c_print('Enter Prisma Cloud Credentials', color='blue')
                 print()
-                name, _id, secret, url, verify, project_flag = __get_config()
+                name, _id, secret, url, verify, proxies, project_flag = __get_config()
                 
-                valid = __universal_validate_credentials(name, url, _id, secret, verify)
+                valid = __universal_validate_credentials(name, url, _id, secret, verify, proxies)
                 if valid == False:
                     __c_print('FAILED', end=' ', color='red')
                     print('Invalid credentials. Please re-enter your credentials')
                     print()
                 else:
-                    credentials.append(__build_config_json(name, _id, secret, url, verify, project_flag))
+                    credentials.append(__build_config_json(name, _id, secret, url, verify, proxies, project_flag))
                     tenant_count +=1
             
             if tenant_count >= min_tenants:
                 __c_print('Would you like to add another Prisma Cloud credential? Y/N')
                 choice = input().lower()
                 if choice != 'yes' and choice != 'y':
                     break
     else:
         while True:
             valid = False
             while not valid:
                 __c_print('Enter Prisma Cloud Credentials', color='blue')
                 print()
-                name, _id, secret, url, verify, project_flag = __get_config()
+                name, _id, secret, url, verify, proxies, project_flag = __get_config()
                 
-                valid = __universal_validate_credentials(name, url, _id, secret, verify)
+                valid = __universal_validate_credentials(name, url, _id, secret, verify, proxies)
                 if valid == False:
                     __c_print('FAILED', end=' ', color='red')
                     print('Invalid credentials. Please re-enter your credentials')
                     print()
                 else:
-                    credentials.append(__build_config_json(name, _id, secret, url, verify, project_flag))
+                    credentials.append(__build_config_json(name, _id, secret, url, verify, proxies, project_flag))
             
             __c_print('Would you like to add another Prisma Cloud credential? Y/N')
             choice = input().lower()
 
             if choice != 'yes' and choice != 'y':
                 break
 
@@ -616,14 +676,15 @@
         verify = os.environ['PC_API_VERIFY']
         if verify.lower() == 'false':
             verify = False
         if verify.lower() == 'true':
             verify = True
     except:
         logger.warning('Missing \'PC_API_VERIFY\' environment variable. Using default value...')
+    
 
     if error_exit:
         logger.info('Missing required environment variables. Exiting...')
         exit()
 
     return CWPSessionManager(name, api_url, uname, passwd, verify, False, logger)
 
@@ -1016,24 +1077,30 @@
         if verify.lower().strip() == 'false':
             verify = False
         elif verify.lower().strip() == 'true':
             verify = True
         else:
             verify = verify
 
+        proxies = None
+        try:
+            proxies = blob['proxies']
+        except:
+            pass    
+
         if 'prismacloud.io' in blob['url'] or 'prismacloud.cn' in blob['url']:
-            tenant_sessions.append(SaaSSessionManager(blob['name'], blob['identity'], blob['secret'], blob['url'], verify, logger=logger))
+            tenant_sessions.append(SaaSSessionManager(blob['name'], blob['identity'], blob['secret'], blob['url'], verify, proxies, logger=logger))
         else:
             project_flag = False
             project_flag_in = blob.get('project_flag', None)
             if project_flag_in:
                 if project_flag_in.lower().strip() == 'true':
                     project_flag = True
 
-            tenant_sessions.append(CWPSessionManager(blob['name'], blob['url'], blob['identity'], blob['secret'], verify, project_flag, logger=logger))
+            tenant_sessions.append(CWPSessionManager(blob['name'], blob['url'], blob['identity'], blob['secret'], verify, proxies, project_flag, logger=logger))
 
     return tenant_sessions
 
 def load_config_user(num_tenants=-1, min_tenants=-1, logger=py_logger):
     if num_tenants != -1 and min_tenants != -1:
         logger.error('ERROR: Incompatible options. Exiting...')
         exit()
@@ -1051,15 +1118,15 @@
             if project_flag_in:
                 if project_flag_in.lower().strip() == 'true':
                     project_flag = True
             tenant_sessions.append(CWPSessionManager(tenant['name'], tenant['url'], tenant['identity'], tenant['secret'], tenant['verify'], project_flag, logger=logger))
 
     return tenant_sessions
 
-def load_config_env(prisma_name='PRISMA_PCPI_NAME', identifier_name='PRISMA_PCPI_ID', secret_name='PRISMA_PCPI_SECRET', api_url_name='PRISMA_PCPI_URL', verify_name='PRISMA_PCPI_VERIFY', project_flag_name='PRISMA_PCPI_PROJECT_FLAG',  logger=py_logger):
+def load_config_env(prisma_name='PRISMA_PCPI_NAME', identifier_name='PRISMA_PCPI_ID', secret_name='PRISMA_PCPI_SECRET', api_url_name='PRISMA_PCPI_URL', verify_name='PRISMA_PCPI_VERIFY', http_name='PC_HTTP_PROXY', https_name='PC_HTTPS_PROXY', project_flag_name='PRISMA_PCPI_PROJECT_FLAG',  logger=py_logger):
     error_exit = False
 
     name = 'Tenant'
     try:
         name = os.environ[prisma_name]
     except:
         logger.warning(f'Missing \'{prisma_name}\' environment variable. Using default name.')
@@ -1091,25 +1158,44 @@
     try:
         verify = os.environ[verify_name]
         if verify.lower() == 'false':
             verify = False
         if verify.lower() == 'true':
             verify = True
     except:
-        logger.warning(f'Missing \'{verify_name}\' environment variable. Using default value...')
+        logger.warning(f'\'{verify_name}\' not set. Using default value...')
+
+    proxies = None
+    http_proxy = None
+    https_proxy = None
+    try:
+        http_proxy = os.environ[http_name]
+    except:
+        logger.warning(f'\'{http_name}\' not set. No HTTP proxy will be used.')
+
+    try:
+        https_proxy = os.environ[https_name]
+    except:
+        logger.warning(f'\'{https_name}\' not set. No HTTPS proxy will be used.')
+
+    if http_proxy or https_proxy:
+        proxies = {
+            'http': http_proxy,
+            'https': https_proxy
+        }
     
     project_flag =  False
     try:
         project_flag = os.environ[project_flag_name]
         if project_flag.lower().strip() == 'true':
             project_flag = True
     except:
-        logger.warning(f'Missing \'{project_flag_name}\' environment variable. Using default value...')
+        logger.warning(f'\'{project_flag_name}\' not set. Using default value...')
 
     if error_exit:
         logger.info('Missing required environment variables. Exiting...')
         exit()
 
     if 'prismacloud.io' in api or 'prismacloud.cn' in api:
-        return SaaSSessionManager(name, a_key, s_key, api, verify, logger=logger)
+        return SaaSSessionManager(name, a_key, s_key, api, verify, proxies, logger=logger)
     else:
-        return CWPSessionManager(name, api, a_key, s_key, verify, project_flag, logger=logger)
+        return CWPSessionManager(name, api, a_key, s_key, verify, proxies, project_flag, logger=logger)
```

### Comparing `pcpi-0.7.0/.gitignore` & `pcpi-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pcpi-0.7.0/LICENSE` & `pcpi-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pcpi-0.7.0/README.md` & `pcpi-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -138,21 +138,19 @@
                 api_url_name='PRISMA_PCPI_URL', verify_name='PRISMA_PCPI_VERIFY',  project_flag_name='PRISMA_PCPI_PROJECT_FLAG', logger=py_logger) # returns single session manager
 
 #-- SESSION MANAGERS --
 #Session loader returns a list of session managers
 session_managers = session_loader.load_config() 
 #load_config() returns either a SaaS session manager or On-Prem session manager based on credentials used, namely the api url.
 my_session_manager = session_managers[0]
-my_onprem_session_manager = session_managers[1]
 
 #Session managers return session objects
 #-- SESSION MANAGER FUNCTIONS --
 cspm_session = my_session_manager.create_cspm_session()
 cwp_session = my_session_manager.create_cwp_session()
-onprem_cwp_session = my_onprem_session_manager.create_cwp_session()
 
 #-- SESSION FUNCTION --
 #Session objects are used to make API requests
 cspm_session.request('GET', '<api_endpoint>', json={}, params={}, verify=True)
 cwp_session.request( 'POST', '<api_endpoint>', json={}, params={}, verify=True)
 
 #-- SESSION REQUEST ARGUMENTS --
@@ -284,21 +282,21 @@
 )
 
 cspm_session = session_manager.create_cspm_session()
 cwp_session = session_manager.create_cwp_session()
 ```
 
 ```python
-from pcpi import onprem_session_manager
+from pcpi import session_manager
 import logging
 
 py_logger = logging.getLogger()
 py_logger.setLevel(10)
 
-session_manager = onprem_session_manager.CWPSessionManager(
+session_manager = session_manager.CWPSessionManager(
     tenant_name='My PC Tenant',
     uname='xxxxxxxxxxxxxxxxxxxxxxxxxx',
     passwd='xxxxxxxxxxxxxxxxxxxxxxxxxx',
     api_url='https://<yourselfhostedurl>',
     logger=py_logger
 )
```

### Comparing `pcpi-0.7.0/pyproject.toml` & `pcpi-0.8.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pcpi"
-version = "0.7.0"
+version = "0.8.0"
 authors = [
   { name="Adam Hamilton-Sutherland", email="ahamiltonsut@paloaltonetworks.com" },
 ]
 description = "Python Package for making API calls to the Prisma Cloud API using best practices."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `pcpi-0.7.0/PKG-INFO` & `pcpi-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcpi
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python Package for making API calls to the Prisma Cloud API using best practices.
 Project-URL: Homepage, https://github.com/PaloAltoNetworks/pc-python-integration
 Project-URL: Bug Tracker, https://github.com/PaloAltoNetworks/pc-python-integration/issues
 Author-email: Adam Hamilton-Sutherland <ahamiltonsut@paloaltonetworks.com>
 License: ISC License
         
         Copyright (c) 2020, Palo Alto Networks Inc.
@@ -170,21 +170,19 @@
                 api_url_name='PRISMA_PCPI_URL', verify_name='PRISMA_PCPI_VERIFY',  project_flag_name='PRISMA_PCPI_PROJECT_FLAG', logger=py_logger) # returns single session manager
 
 #-- SESSION MANAGERS --
 #Session loader returns a list of session managers
 session_managers = session_loader.load_config() 
 #load_config() returns either a SaaS session manager or On-Prem session manager based on credentials used, namely the api url.
 my_session_manager = session_managers[0]
-my_onprem_session_manager = session_managers[1]
 
 #Session managers return session objects
 #-- SESSION MANAGER FUNCTIONS --
 cspm_session = my_session_manager.create_cspm_session()
 cwp_session = my_session_manager.create_cwp_session()
-onprem_cwp_session = my_onprem_session_manager.create_cwp_session()
 
 #-- SESSION FUNCTION --
 #Session objects are used to make API requests
 cspm_session.request('GET', '<api_endpoint>', json={}, params={}, verify=True)
 cwp_session.request( 'POST', '<api_endpoint>', json={}, params={}, verify=True)
 
 #-- SESSION REQUEST ARGUMENTS --
@@ -316,21 +314,21 @@
 )
 
 cspm_session = session_manager.create_cspm_session()
 cwp_session = session_manager.create_cwp_session()
 ```
 
 ```python
-from pcpi import onprem_session_manager
+from pcpi import session_manager
 import logging
 
 py_logger = logging.getLogger()
 py_logger.setLevel(10)
 
-session_manager = onprem_session_manager.CWPSessionManager(
+session_manager = session_manager.CWPSessionManager(
     tenant_name='My PC Tenant',
     uname='xxxxxxxxxxxxxxxxxxxxxxxxxx',
     passwd='xxxxxxxxxxxxxxxxxxxxxxxxxx',
     api_url='https://<yourselfhostedurl>',
     logger=py_logger
 )
```

