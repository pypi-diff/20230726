# Comparing `tmp/alibabacloud_resourcedirectorymaster20220419-1.0.2.tar.gz` & `tmp/alibabacloud_resourcedirectorymaster20220419-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419-1.0.2.tar", last modified: Thu May  4 11:31:56 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419-1.0.3.tar", last modified: Wed Jul 26 01:44:40 2023, max compression
```

## Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.2.tar` & `alibabacloud_resourcedirectorymaster20220419-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2448 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1082 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1167 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   226837 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/client.py
--rw-r--r--   0 root         (0) root         (0)   368465 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2448 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2710 2023-05-04 11:31:56.000000 alibabacloud_resourcedirectorymaster20220419-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   254005 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/client.py
+-rw-r--r--   0 root         (0) root         (0)   404794 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-26 01:44:40.000000 alibabacloud_resourcedirectorymaster20220419-1.0.3/setup.py
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.2/LICENSE` & `alibabacloud_resourcedirectorymaster20220419-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.2/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcedirectorymaster20220419
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.2/README-CN.md` & `alibabacloud_resourcedirectorymaster20220419-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.2/README.md` & `alibabacloud_resourcedirectorymaster20220419-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/client.py` & `alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,14 +42,21 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def accept_handshake_with_options(
         self,
         request: resource_directory_master_20220419_models.AcceptHandshakeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.AcceptHandshakeResponse:
+        """
+        After an invited Alibaba Cloud account joins a resource directory, it becomes a member of the resource directory. By default, the name of the invited Alibaba Cloud account is used as the display name of the account in the resource directory.
+        
+        @param request: AcceptHandshakeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AcceptHandshakeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.handshake_id):
             query['HandshakeId'] = request.handshake_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -70,14 +77,21 @@
         )
 
     async def accept_handshake_with_options_async(
         self,
         request: resource_directory_master_20220419_models.AcceptHandshakeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.AcceptHandshakeResponse:
+        """
+        After an invited Alibaba Cloud account joins a resource directory, it becomes a member of the resource directory. By default, the name of the invited Alibaba Cloud account is used as the display name of the account in the resource directory.
+        
+        @param request: AcceptHandshakeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AcceptHandshakeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.handshake_id):
             query['HandshakeId'] = request.handshake_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -97,21 +111,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def accept_handshake(
         self,
         request: resource_directory_master_20220419_models.AcceptHandshakeRequest,
     ) -> resource_directory_master_20220419_models.AcceptHandshakeResponse:
+        """
+        After an invited Alibaba Cloud account joins a resource directory, it becomes a member of the resource directory. By default, the name of the invited Alibaba Cloud account is used as the display name of the account in the resource directory.
+        
+        @param request: AcceptHandshakeRequest
+        @return: AcceptHandshakeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.accept_handshake_with_options(request, runtime)
 
     async def accept_handshake_async(
         self,
         request: resource_directory_master_20220419_models.AcceptHandshakeRequest,
     ) -> resource_directory_master_20220419_models.AcceptHandshakeResponse:
+        """
+        After an invited Alibaba Cloud account joins a resource directory, it becomes a member of the resource directory. By default, the name of the invited Alibaba Cloud account is used as the display name of the account in the resource directory.
+        
+        @param request: AcceptHandshakeRequest
+        @return: AcceptHandshakeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.accept_handshake_with_options_async(request, runtime)
 
     def add_message_contact_with_options(
         self,
         request: resource_directory_master_20220419_models.AddMessageContactRequest,
         runtime: util_models.RuntimeOptions,
@@ -273,15 +299,18 @@
 
     def attach_control_policy_with_options(
         self,
         request: resource_directory_master_20220419_models.AttachControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.AttachControlPolicyResponse:
         """
-        The ID of the request.
+        After you attach a custom access control policy, the operations performed on resources by using members are limited by the policy. Make sure that the attached policy meets your expectations. Otherwise, your business may be affected.
+        By default, the system access control policy FullAliyunAccess is attached to each folder and member.
+        The access control policy that is attached to a folder also applies to all its subfolders and all members in the subfolders.
+        A maximum of 10 access control policies can be attached to a folder or member.
         
         @param request: AttachControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AttachControlPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -310,15 +339,18 @@
 
     async def attach_control_policy_with_options_async(
         self,
         request: resource_directory_master_20220419_models.AttachControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.AttachControlPolicyResponse:
         """
-        The ID of the request.
+        After you attach a custom access control policy, the operations performed on resources by using members are limited by the policy. Make sure that the attached policy meets your expectations. Otherwise, your business may be affected.
+        By default, the system access control policy FullAliyunAccess is attached to each folder and member.
+        The access control policy that is attached to a folder also applies to all its subfolders and all members in the subfolders.
+        A maximum of 10 access control policies can be attached to a folder or member.
         
         @param request: AttachControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: AttachControlPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -346,42 +378,49 @@
         )
 
     def attach_control_policy(
         self,
         request: resource_directory_master_20220419_models.AttachControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.AttachControlPolicyResponse:
         """
-        The ID of the request.
+        After you attach a custom access control policy, the operations performed on resources by using members are limited by the policy. Make sure that the attached policy meets your expectations. Otherwise, your business may be affected.
+        By default, the system access control policy FullAliyunAccess is attached to each folder and member.
+        The access control policy that is attached to a folder also applies to all its subfolders and all members in the subfolders.
+        A maximum of 10 access control policies can be attached to a folder or member.
         
         @param request: AttachControlPolicyRequest
         @return: AttachControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.attach_control_policy_with_options(request, runtime)
 
     async def attach_control_policy_async(
         self,
         request: resource_directory_master_20220419_models.AttachControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.AttachControlPolicyResponse:
         """
-        The ID of the request.
+        After you attach a custom access control policy, the operations performed on resources by using members are limited by the policy. Make sure that the attached policy meets your expectations. Otherwise, your business may be affected.
+        By default, the system access control policy FullAliyunAccess is attached to each folder and member.
+        The access control policy that is attached to a folder also applies to all its subfolders and all members in the subfolders.
+        A maximum of 10 access control policies can be attached to a folder or member.
         
         @param request: AttachControlPolicyRequest
         @return: AttachControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.attach_control_policy_with_options_async(request, runtime)
 
     def bind_secure_mobile_phone_with_options(
         self,
         request: resource_directory_master_20220419_models.BindSecureMobilePhoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.BindSecureMobilePhoneResponse:
         """
-        The ID of the request.
+        You can call this API operation only to bind a mobile phone number to a member of the resource account type. You cannot call this API operation to change the mobile phone number that is bound to a member of the resource account type.
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this API operation.
         
         @param request: BindSecureMobilePhoneRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BindSecureMobilePhoneResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -412,15 +451,16 @@
 
     async def bind_secure_mobile_phone_with_options_async(
         self,
         request: resource_directory_master_20220419_models.BindSecureMobilePhoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.BindSecureMobilePhoneResponse:
         """
-        The ID of the request.
+        You can call this API operation only to bind a mobile phone number to a member of the resource account type. You cannot call this API operation to change the mobile phone number that is bound to a member of the resource account type.
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this API operation.
         
         @param request: BindSecureMobilePhoneRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BindSecureMobilePhoneResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -450,28 +490,30 @@
         )
 
     def bind_secure_mobile_phone(
         self,
         request: resource_directory_master_20220419_models.BindSecureMobilePhoneRequest,
     ) -> resource_directory_master_20220419_models.BindSecureMobilePhoneResponse:
         """
-        The ID of the request.
+        You can call this API operation only to bind a mobile phone number to a member of the resource account type. You cannot call this API operation to change the mobile phone number that is bound to a member of the resource account type.
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this API operation.
         
         @param request: BindSecureMobilePhoneRequest
         @return: BindSecureMobilePhoneResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.bind_secure_mobile_phone_with_options(request, runtime)
 
     async def bind_secure_mobile_phone_async(
         self,
         request: resource_directory_master_20220419_models.BindSecureMobilePhoneRequest,
     ) -> resource_directory_master_20220419_models.BindSecureMobilePhoneResponse:
         """
-        The ID of the request.
+        You can call this API operation only to bind a mobile phone number to a member of the resource account type. You cannot call this API operation to change the mobile phone number that is bound to a member of the resource account type.
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this API operation.
         
         @param request: BindSecureMobilePhoneRequest
         @return: BindSecureMobilePhoneResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.bind_secure_mobile_phone_with_options_async(request, runtime)
 
@@ -769,15 +811,15 @@
 
     def check_account_delete_with_options(
         self,
         request: resource_directory_master_20220419_models.CheckAccountDeleteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CheckAccountDeleteResponse:
         """
-        The returned result.
+        Before you delete a member, you must call this API operation to check whether the member can be deleted.
         
         @param request: CheckAccountDeleteRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CheckAccountDeleteResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -804,15 +846,15 @@
 
     async def check_account_delete_with_options_async(
         self,
         request: resource_directory_master_20220419_models.CheckAccountDeleteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CheckAccountDeleteResponse:
         """
-        The returned result.
+        Before you delete a member, you must call this API operation to check whether the member can be deleted.
         
         @param request: CheckAccountDeleteRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CheckAccountDeleteResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -838,28 +880,28 @@
         )
 
     def check_account_delete(
         self,
         request: resource_directory_master_20220419_models.CheckAccountDeleteRequest,
     ) -> resource_directory_master_20220419_models.CheckAccountDeleteResponse:
         """
-        The returned result.
+        Before you delete a member, you must call this API operation to check whether the member can be deleted.
         
         @param request: CheckAccountDeleteRequest
         @return: CheckAccountDeleteResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.check_account_delete_with_options(request, runtime)
 
     async def check_account_delete_async(
         self,
         request: resource_directory_master_20220419_models.CheckAccountDeleteRequest,
     ) -> resource_directory_master_20220419_models.CheckAccountDeleteResponse:
         """
-        The returned result.
+        Before you delete a member, you must call this API operation to check whether the member can be deleted.
         
         @param request: CheckAccountDeleteRequest
         @return: CheckAccountDeleteResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.check_account_delete_with_options_async(request, runtime)
 
@@ -947,15 +989,15 @@
 
     def create_folder_with_options(
         self,
         request: resource_directory_master_20220419_models.CreateFolderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CreateFolderResponse:
         """
-        The name of the folder.
+        A maximum of five levels of folders can be created under the Root folder.
         
         @param request: CreateFolderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateFolderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -984,15 +1026,15 @@
 
     async def create_folder_with_options_async(
         self,
         request: resource_directory_master_20220419_models.CreateFolderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CreateFolderResponse:
         """
-        The name of the folder.
+        A maximum of five levels of folders can be created under the Root folder.
         
         @param request: CreateFolderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateFolderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1020,42 +1062,43 @@
         )
 
     def create_folder(
         self,
         request: resource_directory_master_20220419_models.CreateFolderRequest,
     ) -> resource_directory_master_20220419_models.CreateFolderResponse:
         """
-        The name of the folder.
+        A maximum of five levels of folders can be created under the Root folder.
         
         @param request: CreateFolderRequest
         @return: CreateFolderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_folder_with_options(request, runtime)
 
     async def create_folder_async(
         self,
         request: resource_directory_master_20220419_models.CreateFolderRequest,
     ) -> resource_directory_master_20220419_models.CreateFolderResponse:
         """
-        The name of the folder.
+        A maximum of five levels of folders can be created under the Root folder.
         
         @param request: CreateFolderRequest
         @return: CreateFolderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_folder_with_options_async(request, runtime)
 
     def create_resource_account_with_options(
         self,
         request: resource_directory_master_20220419_models.CreateResourceAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CreateResourceAccountResponse:
         """
-        The Alibaba Cloud account name of the member.
+        A member serves as a container for resources and is also an organizational unit in a resource directory. A member indicates a project or application. The resources of different members are isolated.
+        This topic provides an example on how to call the API operation to create a member in the `fd-r23M55****` folder. The display name of the member is `Dev`, and the prefix for the Alibaba Cloud account name of the member is `alice`.
         
         @param request: CreateResourceAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateResourceAccountResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1092,15 +1135,16 @@
 
     async def create_resource_account_with_options_async(
         self,
         request: resource_directory_master_20220419_models.CreateResourceAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.CreateResourceAccountResponse:
         """
-        The Alibaba Cloud account name of the member.
+        A member serves as a container for resources and is also an organizational unit in a resource directory. A member indicates a project or application. The resources of different members are isolated.
+        This topic provides an example on how to call the API operation to create a member in the `fd-r23M55****` folder. The display name of the member is `Dev`, and the prefix for the Alibaba Cloud account name of the member is `alice`.
         
         @param request: CreateResourceAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateResourceAccountResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1136,28 +1180,30 @@
         )
 
     def create_resource_account(
         self,
         request: resource_directory_master_20220419_models.CreateResourceAccountRequest,
     ) -> resource_directory_master_20220419_models.CreateResourceAccountResponse:
         """
-        The Alibaba Cloud account name of the member.
+        A member serves as a container for resources and is also an organizational unit in a resource directory. A member indicates a project or application. The resources of different members are isolated.
+        This topic provides an example on how to call the API operation to create a member in the `fd-r23M55****` folder. The display name of the member is `Dev`, and the prefix for the Alibaba Cloud account name of the member is `alice`.
         
         @param request: CreateResourceAccountRequest
         @return: CreateResourceAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_resource_account_with_options(request, runtime)
 
     async def create_resource_account_async(
         self,
         request: resource_directory_master_20220419_models.CreateResourceAccountRequest,
     ) -> resource_directory_master_20220419_models.CreateResourceAccountResponse:
         """
-        The Alibaba Cloud account name of the member.
+        A member serves as a container for resources and is also an organizational unit in a resource directory. A member indicates a project or application. The resources of different members are isolated.
+        This topic provides an example on how to call the API operation to create a member in the `fd-r23M55****` folder. The display name of the member is `Dev`, and the prefix for the Alibaba Cloud account name of the member is `alice`.
         
         @param request: CreateResourceAccountRequest
         @return: CreateResourceAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_resource_account_with_options_async(request, runtime)
 
@@ -1232,14 +1278,23 @@
         return await self.decline_handshake_with_options_async(request, runtime)
 
     def delete_account_with_options(
         self,
         tmp_req: resource_directory_master_20220419_models.DeleteAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
+        """
+        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
+        Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
+        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
+        
+        @param tmp_req: DeleteAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAccountResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = resource_directory_master_20220419_models.DeleteAccountShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.abandonable_check_id):
             request.abandonable_check_id_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.abandonable_check_id, 'AbandonableCheckId', 'json')
         query = {}
         if not UtilClient.is_unset(request.abandonable_check_id_shrink):
@@ -1266,14 +1321,23 @@
         )
 
     async def delete_account_with_options_async(
         self,
         tmp_req: resource_directory_master_20220419_models.DeleteAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
+        """
+        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
+        Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
+        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
+        
+        @param tmp_req: DeleteAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAccountResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = resource_directory_master_20220419_models.DeleteAccountShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.abandonable_check_id):
             request.abandonable_check_id_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.abandonable_check_id, 'AbandonableCheckId', 'json')
         query = {}
         if not UtilClient.is_unset(request.abandonable_check_id_shrink):
@@ -1299,31 +1363,47 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_account(
         self,
         request: resource_directory_master_20220419_models.DeleteAccountRequest,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
+        """
+        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
+        Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
+        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
+        
+        @param request: DeleteAccountRequest
+        @return: DeleteAccountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_account_with_options(request, runtime)
 
     async def delete_account_async(
         self,
         request: resource_directory_master_20220419_models.DeleteAccountRequest,
     ) -> resource_directory_master_20220419_models.DeleteAccountResponse:
+        """
+        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
+        Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
+        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
+        
+        @param request: DeleteAccountRequest
+        @return: DeleteAccountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_account_with_options_async(request, runtime)
 
     def delete_control_policy_with_options(
         self,
         request: resource_directory_master_20220419_models.DeleteControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteControlPolicyResponse:
         """
-        The ID of the request.
+        If you want to delete a custom access control policy that is attached to folders or members, you must call the [DetachControlPolicy](~~DetachControlPolicy~~) operation to detach the policy before you delete it.
         
         @param request: DeleteControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteControlPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1350,15 +1430,15 @@
 
     async def delete_control_policy_with_options_async(
         self,
         request: resource_directory_master_20220419_models.DeleteControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteControlPolicyResponse:
         """
-        The ID of the request.
+        If you want to delete a custom access control policy that is attached to folders or members, you must call the [DetachControlPolicy](~~DetachControlPolicy~~) operation to detach the policy before you delete it.
         
         @param request: DeleteControlPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteControlPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1384,42 +1464,42 @@
         )
 
     def delete_control_policy(
         self,
         request: resource_directory_master_20220419_models.DeleteControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.DeleteControlPolicyResponse:
         """
-        The ID of the request.
+        If you want to delete a custom access control policy that is attached to folders or members, you must call the [DetachControlPolicy](~~DetachControlPolicy~~) operation to detach the policy before you delete it.
         
         @param request: DeleteControlPolicyRequest
         @return: DeleteControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_control_policy_with_options(request, runtime)
 
     async def delete_control_policy_async(
         self,
         request: resource_directory_master_20220419_models.DeleteControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.DeleteControlPolicyResponse:
         """
-        The ID of the request.
+        If you want to delete a custom access control policy that is attached to folders or members, you must call the [DetachControlPolicy](~~DetachControlPolicy~~) operation to detach the policy before you delete it.
         
         @param request: DeleteControlPolicyRequest
         @return: DeleteControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_control_policy_with_options_async(request, runtime)
 
     def delete_folder_with_options(
         self,
         request: resource_directory_master_20220419_models.DeleteFolderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteFolderResponse:
         """
-        The ID of the request.
+        Before you delete a folder, you must make sure that the folder does not contain members or subfolders.
         
         @param request: DeleteFolderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteFolderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1446,15 +1526,15 @@
 
     async def delete_folder_with_options_async(
         self,
         request: resource_directory_master_20220419_models.DeleteFolderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeleteFolderResponse:
         """
-        The ID of the request.
+        Before you delete a folder, you must make sure that the folder does not contain members or subfolders.
         
         @param request: DeleteFolderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteFolderResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1480,28 +1560,28 @@
         )
 
     def delete_folder(
         self,
         request: resource_directory_master_20220419_models.DeleteFolderRequest,
     ) -> resource_directory_master_20220419_models.DeleteFolderResponse:
         """
-        The ID of the request.
+        Before you delete a folder, you must make sure that the folder does not contain members or subfolders.
         
         @param request: DeleteFolderRequest
         @return: DeleteFolderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_folder_with_options(request, runtime)
 
     async def delete_folder_async(
         self,
         request: resource_directory_master_20220419_models.DeleteFolderRequest,
     ) -> resource_directory_master_20220419_models.DeleteFolderResponse:
         """
-        The ID of the request.
+        Before you delete a folder, you must make sure that the folder does not contain members or subfolders.
         
         @param request: DeleteFolderRequest
         @return: DeleteFolderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_folder_with_options_async(request, runtime)
 
@@ -1580,14 +1660,21 @@
         return await self.delete_message_contact_with_options_async(request, runtime)
 
     def deregister_delegated_administrator_with_options(
         self,
         request: resource_directory_master_20220419_models.DeregisterDelegatedAdministratorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeregisterDelegatedAdministratorResponse:
+        """
+        If the delegated administrator account that you want to remove has historical management tasks in the related trusted service, the trusted service may be affected after the delegated administrator account is removed. Therefore, proceed with caution.
+        
+        @param request: DeregisterDelegatedAdministratorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeregisterDelegatedAdministratorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.service_principal):
             query['ServicePrincipal'] = request.service_principal
         req = open_api_models.OpenApiRequest(
@@ -1610,14 +1697,21 @@
         )
 
     async def deregister_delegated_administrator_with_options_async(
         self,
         request: resource_directory_master_20220419_models.DeregisterDelegatedAdministratorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DeregisterDelegatedAdministratorResponse:
+        """
+        If the delegated administrator account that you want to remove has historical management tasks in the related trusted service, the trusted service may be affected after the delegated administrator account is removed. Therefore, proceed with caution.
+        
+        @param request: DeregisterDelegatedAdministratorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeregisterDelegatedAdministratorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.service_principal):
             query['ServicePrincipal'] = request.service_principal
         req = open_api_models.OpenApiRequest(
@@ -1639,21 +1733,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def deregister_delegated_administrator(
         self,
         request: resource_directory_master_20220419_models.DeregisterDelegatedAdministratorRequest,
     ) -> resource_directory_master_20220419_models.DeregisterDelegatedAdministratorResponse:
+        """
+        If the delegated administrator account that you want to remove has historical management tasks in the related trusted service, the trusted service may be affected after the delegated administrator account is removed. Therefore, proceed with caution.
+        
+        @param request: DeregisterDelegatedAdministratorRequest
+        @return: DeregisterDelegatedAdministratorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.deregister_delegated_administrator_with_options(request, runtime)
 
     async def deregister_delegated_administrator_async(
         self,
         request: resource_directory_master_20220419_models.DeregisterDelegatedAdministratorRequest,
     ) -> resource_directory_master_20220419_models.DeregisterDelegatedAdministratorResponse:
+        """
+        If the delegated administrator account that you want to remove has historical management tasks in the related trusted service, the trusted service may be affected after the delegated administrator account is removed. Therefore, proceed with caution.
+        
+        @param request: DeregisterDelegatedAdministratorRequest
+        @return: DeregisterDelegatedAdministratorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.deregister_delegated_administrator_with_options_async(request, runtime)
 
     def destroy_resource_directory_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DestroyResourceDirectoryResponse:
@@ -1728,14 +1834,22 @@
         return await self.destroy_resource_directory_with_options_async(runtime)
 
     def detach_control_policy_with_options(
         self,
         request: resource_directory_master_20220419_models.DetachControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DetachControlPolicyResponse:
+        """
+        After you detach an access control policy, the operations performed on resources by using members are not limited by the policy. Make sure that the detached policy meets your expectations. Otherwise, your business may be affected.
+        Both the system and custom access control policies can be detached. If an object has only one access control policy attached, the policy cannot be detached.
+        
+        @param request: DetachControlPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetachControlPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.policy_id):
             query['PolicyId'] = request.policy_id
         if not UtilClient.is_unset(request.target_id):
             query['TargetId'] = request.target_id
         req = open_api_models.OpenApiRequest(
@@ -1758,14 +1872,22 @@
         )
 
     async def detach_control_policy_with_options_async(
         self,
         request: resource_directory_master_20220419_models.DetachControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DetachControlPolicyResponse:
+        """
+        After you detach an access control policy, the operations performed on resources by using members are not limited by the policy. Make sure that the detached policy meets your expectations. Otherwise, your business may be affected.
+        Both the system and custom access control policies can be detached. If an object has only one access control policy attached, the policy cannot be detached.
+        
+        @param request: DetachControlPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetachControlPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.policy_id):
             query['PolicyId'] = request.policy_id
         if not UtilClient.is_unset(request.target_id):
             query['TargetId'] = request.target_id
         req = open_api_models.OpenApiRequest(
@@ -1787,21 +1909,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def detach_control_policy(
         self,
         request: resource_directory_master_20220419_models.DetachControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.DetachControlPolicyResponse:
+        """
+        After you detach an access control policy, the operations performed on resources by using members are not limited by the policy. Make sure that the detached policy meets your expectations. Otherwise, your business may be affected.
+        Both the system and custom access control policies can be detached. If an object has only one access control policy attached, the policy cannot be detached.
+        
+        @param request: DetachControlPolicyRequest
+        @return: DetachControlPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.detach_control_policy_with_options(request, runtime)
 
     async def detach_control_policy_async(
         self,
         request: resource_directory_master_20220419_models.DetachControlPolicyRequest,
     ) -> resource_directory_master_20220419_models.DetachControlPolicyResponse:
+        """
+        After you detach an access control policy, the operations performed on resources by using members are not limited by the policy. Make sure that the detached policy meets your expectations. Otherwise, your business may be affected.
+        Both the system and custom access control policies can be detached. If an object has only one access control policy attached, the policy cannot be detached.
+        
+        @param request: DetachControlPolicyRequest
+        @return: DetachControlPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.detach_control_policy_with_options_async(request, runtime)
 
     def disable_control_policy_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.DisableControlPolicyResponse:
@@ -2025,15 +2161,15 @@
 
     def enable_resource_directory_with_options(
         self,
         request: resource_directory_master_20220419_models.EnableResourceDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.EnableResourceDirectoryResponse:
         """
-        The ID of the request.
+        You can use the current account or a newly created account to enable a resource directory. For more information, see [Enable a resource directory](~~111215~~).
         
         @param request: EnableResourceDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: EnableResourceDirectoryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2066,15 +2202,15 @@
 
     async def enable_resource_directory_with_options_async(
         self,
         request: resource_directory_master_20220419_models.EnableResourceDirectoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.EnableResourceDirectoryResponse:
         """
-        The ID of the request.
+        You can use the current account or a newly created account to enable a resource directory. For more information, see [Enable a resource directory](~~111215~~).
         
         @param request: EnableResourceDirectoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: EnableResourceDirectoryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2106,28 +2242,28 @@
         )
 
     def enable_resource_directory(
         self,
         request: resource_directory_master_20220419_models.EnableResourceDirectoryRequest,
     ) -> resource_directory_master_20220419_models.EnableResourceDirectoryResponse:
         """
-        The ID of the request.
+        You can use the current account or a newly created account to enable a resource directory. For more information, see [Enable a resource directory](~~111215~~).
         
         @param request: EnableResourceDirectoryRequest
         @return: EnableResourceDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.enable_resource_directory_with_options(request, runtime)
 
     async def enable_resource_directory_async(
         self,
         request: resource_directory_master_20220419_models.EnableResourceDirectoryRequest,
     ) -> resource_directory_master_20220419_models.EnableResourceDirectoryResponse:
         """
-        The ID of the request.
+        You can use the current account or a newly created account to enable a resource directory. For more information, see [Enable a resource directory](~~111215~~).
         
         @param request: EnableResourceDirectoryRequest
         @return: EnableResourceDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.enable_resource_directory_with_options_async(request, runtime)
 
@@ -2207,15 +2343,15 @@
 
     def get_account_deletion_check_result_with_options(
         self,
         request: resource_directory_master_20220419_models.GetAccountDeletionCheckResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.GetAccountDeletionCheckResultResponse:
         """
-        Container Service for Kubernetes
+        After you call the [CheckAccountDelete](~~CheckAccountDelete~~) operation to perform a member deletion check, you can call the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation to query the check result. If the check result shows that the member meets deletion requirements, you can delete the member. Otherwise, you need to first modify the items that do not meet requirements.
         
         @param request: GetAccountDeletionCheckResultRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAccountDeletionCheckResultResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2242,15 +2378,15 @@
 
     async def get_account_deletion_check_result_with_options_async(
         self,
         request: resource_directory_master_20220419_models.GetAccountDeletionCheckResultRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.GetAccountDeletionCheckResultResponse:
         """
-        Container Service for Kubernetes
+        After you call the [CheckAccountDelete](~~CheckAccountDelete~~) operation to perform a member deletion check, you can call the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation to query the check result. If the check result shows that the member meets deletion requirements, you can delete the member. Otherwise, you need to first modify the items that do not meet requirements.
         
         @param request: GetAccountDeletionCheckResultRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetAccountDeletionCheckResultResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2276,28 +2412,28 @@
         )
 
     def get_account_deletion_check_result(
         self,
         request: resource_directory_master_20220419_models.GetAccountDeletionCheckResultRequest,
     ) -> resource_directory_master_20220419_models.GetAccountDeletionCheckResultResponse:
         """
-        Container Service for Kubernetes
+        After you call the [CheckAccountDelete](~~CheckAccountDelete~~) operation to perform a member deletion check, you can call the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation to query the check result. If the check result shows that the member meets deletion requirements, you can delete the member. Otherwise, you need to first modify the items that do not meet requirements.
         
         @param request: GetAccountDeletionCheckResultRequest
         @return: GetAccountDeletionCheckResultResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_account_deletion_check_result_with_options(request, runtime)
 
     async def get_account_deletion_check_result_async(
         self,
         request: resource_directory_master_20220419_models.GetAccountDeletionCheckResultRequest,
     ) -> resource_directory_master_20220419_models.GetAccountDeletionCheckResultResponse:
         """
-        Container Service for Kubernetes
+        After you call the [CheckAccountDelete](~~CheckAccountDelete~~) operation to perform a member deletion check, you can call the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation to query the check result. If the check result shows that the member meets deletion requirements, you can delete the member. Otherwise, you need to first modify the items that do not meet requirements.
         
         @param request: GetAccountDeletionCheckResultRequest
         @return: GetAccountDeletionCheckResultResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_account_deletion_check_result_with_options_async(request, runtime)
 
@@ -4139,15 +4275,15 @@
 
     def list_trusted_service_status_with_options(
         self,
         request: resource_directory_master_20220419_models.ListTrustedServiceStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.ListTrustedServiceStatusResponse:
         """
-        The time when the trusted service was enabled.
+        Only a management account or delegated administrator account can be used to call this operation.
         
         @param request: ListTrustedServiceStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListTrustedServiceStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4178,15 +4314,15 @@
 
     async def list_trusted_service_status_with_options_async(
         self,
         request: resource_directory_master_20220419_models.ListTrustedServiceStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.ListTrustedServiceStatusResponse:
         """
-        The time when the trusted service was enabled.
+        Only a management account or delegated administrator account can be used to call this operation.
         
         @param request: ListTrustedServiceStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListTrustedServiceStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4216,28 +4352,28 @@
         )
 
     def list_trusted_service_status(
         self,
         request: resource_directory_master_20220419_models.ListTrustedServiceStatusRequest,
     ) -> resource_directory_master_20220419_models.ListTrustedServiceStatusResponse:
         """
-        The time when the trusted service was enabled.
+        Only a management account or delegated administrator account can be used to call this operation.
         
         @param request: ListTrustedServiceStatusRequest
         @return: ListTrustedServiceStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_trusted_service_status_with_options(request, runtime)
 
     async def list_trusted_service_status_async(
         self,
         request: resource_directory_master_20220419_models.ListTrustedServiceStatusRequest,
     ) -> resource_directory_master_20220419_models.ListTrustedServiceStatusResponse:
         """
-        The time when the trusted service was enabled.
+        Only a management account or delegated administrator account can be used to call this operation.
         
         @param request: ListTrustedServiceStatusRequest
         @return: ListTrustedServiceStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_trusted_service_status_with_options_async(request, runtime)
 
@@ -4316,14 +4452,24 @@
         return await self.move_account_with_options_async(request, runtime)
 
     def register_delegated_administrator_with_options(
         self,
         request: resource_directory_master_20220419_models.RegisterDelegatedAdministratorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.RegisterDelegatedAdministratorResponse:
+        """
+        The delegated administrator account can be used to access the information of the resource directory and view the structure and members of the resource directory. The delegated administrator account can also be used to perform service-related management operations in the trusted service on behalf of the management account of the resource directory. When you call this operation, you must take note of the following limits:
+        *   Only some trusted services support delegated administrator accounts. For more information, see [Supported trusted services](~~208133~~).
+        *   Only the management account of a resource directory or an authorized RAM user or RAM role of the management account can be used to call this operation.
+        *   The number of delegated administrator accounts that are allowed for a trusted service is defined by the trusted service.
+        
+        @param request: RegisterDelegatedAdministratorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RegisterDelegatedAdministratorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.service_principal):
             query['ServicePrincipal'] = request.service_principal
         req = open_api_models.OpenApiRequest(
@@ -4346,14 +4492,24 @@
         )
 
     async def register_delegated_administrator_with_options_async(
         self,
         request: resource_directory_master_20220419_models.RegisterDelegatedAdministratorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.RegisterDelegatedAdministratorResponse:
+        """
+        The delegated administrator account can be used to access the information of the resource directory and view the structure and members of the resource directory. The delegated administrator account can also be used to perform service-related management operations in the trusted service on behalf of the management account of the resource directory. When you call this operation, you must take note of the following limits:
+        *   Only some trusted services support delegated administrator accounts. For more information, see [Supported trusted services](~~208133~~).
+        *   Only the management account of a resource directory or an authorized RAM user or RAM role of the management account can be used to call this operation.
+        *   The number of delegated administrator accounts that are allowed for a trusted service is defined by the trusted service.
+        
+        @param request: RegisterDelegatedAdministratorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RegisterDelegatedAdministratorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.service_principal):
             query['ServicePrincipal'] = request.service_principal
         req = open_api_models.OpenApiRequest(
@@ -4375,21 +4531,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def register_delegated_administrator(
         self,
         request: resource_directory_master_20220419_models.RegisterDelegatedAdministratorRequest,
     ) -> resource_directory_master_20220419_models.RegisterDelegatedAdministratorResponse:
+        """
+        The delegated administrator account can be used to access the information of the resource directory and view the structure and members of the resource directory. The delegated administrator account can also be used to perform service-related management operations in the trusted service on behalf of the management account of the resource directory. When you call this operation, you must take note of the following limits:
+        *   Only some trusted services support delegated administrator accounts. For more information, see [Supported trusted services](~~208133~~).
+        *   Only the management account of a resource directory or an authorized RAM user or RAM role of the management account can be used to call this operation.
+        *   The number of delegated administrator accounts that are allowed for a trusted service is defined by the trusted service.
+        
+        @param request: RegisterDelegatedAdministratorRequest
+        @return: RegisterDelegatedAdministratorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.register_delegated_administrator_with_options(request, runtime)
 
     async def register_delegated_administrator_async(
         self,
         request: resource_directory_master_20220419_models.RegisterDelegatedAdministratorRequest,
     ) -> resource_directory_master_20220419_models.RegisterDelegatedAdministratorResponse:
+        """
+        The delegated administrator account can be used to access the information of the resource directory and view the structure and members of the resource directory. The delegated administrator account can also be used to perform service-related management operations in the trusted service on behalf of the management account of the resource directory. When you call this operation, you must take note of the following limits:
+        *   Only some trusted services support delegated administrator accounts. For more information, see [Supported trusted services](~~208133~~).
+        *   Only the management account of a resource directory or an authorized RAM user or RAM role of the management account can be used to call this operation.
+        *   The number of delegated administrator accounts that are allowed for a trusted service is defined by the trusted service.
+        
+        @param request: RegisterDelegatedAdministratorRequest
+        @return: RegisterDelegatedAdministratorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.register_delegated_administrator_with_options_async(request, runtime)
 
     def remove_cloud_account_with_options(
         self,
         request: resource_directory_master_20220419_models.RemoveCloudAccountRequest,
         runtime: util_models.RuntimeOptions,
@@ -5130,14 +5304,23 @@
         return await self.untag_resources_with_options_async(request, runtime)
 
     def update_account_with_options(
         self,
         request: resource_directory_master_20220419_models.UpdateAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.UpdateAccountResponse:
+        """
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this operation.
+        *   Before you switch the type of a member from resource account to cloud account, make sure that specific conditions are met. For more information about the conditions, see [Switch a resource account to a cloud account](~~111233~~).
+        *   Before you switch the type of a member from cloud account to resource account, make sure that specific conditions are met. For more information about the conditions, see [Switch a cloud account to a resource account](~~209980~~).
+        
+        @param request: UpdateAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAccountResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.new_account_type):
             query['NewAccountType'] = request.new_account_type
         if not UtilClient.is_unset(request.new_display_name):
@@ -5162,14 +5345,23 @@
         )
 
     async def update_account_with_options_async(
         self,
         request: resource_directory_master_20220419_models.UpdateAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> resource_directory_master_20220419_models.UpdateAccountResponse:
+        """
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this operation.
+        *   Before you switch the type of a member from resource account to cloud account, make sure that specific conditions are met. For more information about the conditions, see [Switch a resource account to a cloud account](~~111233~~).
+        *   Before you switch the type of a member from cloud account to resource account, make sure that specific conditions are met. For more information about the conditions, see [Switch a cloud account to a resource account](~~209980~~).
+        
+        @param request: UpdateAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAccountResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.new_account_type):
             query['NewAccountType'] = request.new_account_type
         if not UtilClient.is_unset(request.new_display_name):
@@ -5193,21 +5385,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_account(
         self,
         request: resource_directory_master_20220419_models.UpdateAccountRequest,
     ) -> resource_directory_master_20220419_models.UpdateAccountResponse:
+        """
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this operation.
+        *   Before you switch the type of a member from resource account to cloud account, make sure that specific conditions are met. For more information about the conditions, see [Switch a resource account to a cloud account](~~111233~~).
+        *   Before you switch the type of a member from cloud account to resource account, make sure that specific conditions are met. For more information about the conditions, see [Switch a cloud account to a resource account](~~209980~~).
+        
+        @param request: UpdateAccountRequest
+        @return: UpdateAccountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_account_with_options(request, runtime)
 
     async def update_account_async(
         self,
         request: resource_directory_master_20220419_models.UpdateAccountRequest,
     ) -> resource_directory_master_20220419_models.UpdateAccountResponse:
+        """
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this operation.
+        *   Before you switch the type of a member from resource account to cloud account, make sure that specific conditions are met. For more information about the conditions, see [Switch a resource account to a cloud account](~~111233~~).
+        *   Before you switch the type of a member from cloud account to resource account, make sure that specific conditions are met. For more information about the conditions, see [Switch a cloud account to a resource account](~~209980~~).
+        
+        @param request: UpdateAccountRequest
+        @return: UpdateAccountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_account_with_options_async(request, runtime)
 
     def update_control_policy_with_options(
         self,
         request: resource_directory_master_20220419_models.UpdateControlPolicyRequest,
         runtime: util_models.RuntimeOptions,
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419/models.py` & `alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 
 class AcceptHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
+        # The ID of the invitation.
+        # 
+        # You can call the [ListHandshakesForAccount](~~ListHandshakesForAccount~~) operation to obtain the ID.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -42,24 +45,44 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The description of the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status
+        # The ID or logon email address of the invited Alibaba Cloud account.
         self.target_entity = target_entity
+        # The type of the invited Alibaba Cloud account. Valid values:
+        # 
+        # *   Account: indicates the ID of the Alibaba Cloud account.
+        # *   Email: indicates the logon email address of the Alibaba Cloud account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -120,15 +143,17 @@
 
 class AcceptHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: AcceptHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
+        # The information of the invitation.
         self.handshake = handshake
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -202,18 +227,83 @@
         self,
         email_address: str = None,
         message_types: List[str] = None,
         name: str = None,
         phone_number: str = None,
         title: str = None,
     ):
+        # The email address of the contact.
+        # 
+        # After you specify an email address, you need to call [SendEmailVerificationForMessageContact](~~SendEmailVerificationForMessageContact~~) to send verification information to the email address. After the verification is passed, the email address takes effect.
         self.email_address = email_address
+        # The types of messages received by the contact.
         self.message_types = message_types
+        # The name of the contact.
+        # 
+        # The name must be unique in your resource directory.
+        # 
+        # The name must be 2 to 12 characters in length and can contain only letters.
         self.name = name
+        # The mobile phone number of the contact.
+        # 
+        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
+        # 
+        # After you specify a mobile phone number, you need to call [SendPhoneVerificationForMessageContact](~~SendPhoneVerificationForMessageContact~~) to send verification information to the mobile phone number. After the verification is passed, the mobile phone number takes effect.
         self.phone_number = phone_number
+        # The job title of the contact.
+        # 
+        # Valid values:
+        # 
+        # *   FinanceDirector
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   TechnicalDirector
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   MaintenanceDirector
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   CEO
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   ProjectDirector
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   Other
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
         self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -250,15 +340,17 @@
 
 class AddMessageContactResponseBodyContact(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         create_date: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The time when the contact was created.
         self.create_date = create_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -283,15 +375,17 @@
 
 class AddMessageContactResponseBody(TeaModel):
     def __init__(
         self,
         contact: AddMessageContactResponseBodyContact = None,
         request_id: str = None,
     ):
+        # The information about the contact.
         self.contact = contact
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.contact:
             self.contact.validate()
 
     def to_map(self):
@@ -362,15 +456,17 @@
 
 class AssociateMembersRequest(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         members: List[str] = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The IDs of objects to which you want to bind the contact.
         self.members = members
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -396,16 +492,23 @@
 class AssociateMembersResponseBodyMembers(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         member_id: str = None,
         modify_date: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The ID of the object. Valid values:
+        # 
+        # - ID of the resource directory
+        # - ID of the folder
+        # - ID of the member
         self.member_id = member_id
+        # The time when the contact was bound to the object.
         self.modify_date = modify_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -434,15 +537,17 @@
 
 class AssociateMembersResponseBody(TeaModel):
     def __init__(
         self,
         members: List[AssociateMembersResponseBodyMembers] = None,
         request_id: str = None,
     ):
+        # The time when the contact was bound to the object.
         self.members = members
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.members:
             for k in self.members:
                 if k:
                     k.validate()
@@ -519,15 +624,21 @@
 
 class AttachControlPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
         target_id: str = None,
     ):
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The ID of the object to which you want to attach the access control policy. Access control policies can be attached to the following objects:
+        # 
+        # *   Root folder
+        # *   Subfolders of the Root folder
+        # *   Members
         self.target_id = target_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -551,14 +662,15 @@
 
 
 class AttachControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -624,16 +736,27 @@
 class BindSecureMobilePhoneRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         secure_mobile_phone: str = None,
         verification_code: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The mobile phone number that you want to bind to the member for security purposes.
+        # 
+        # The mobile phone number you specify must be the same as the mobile phone number that you specify when you call the [SendVerificationCodeForBindSecureMobilePhone](~~SendVerificationCodeForBindSecureMobilePhone~~) operation to obtain a verification code.
+        # 
+        # Specify the mobile phone number in the \<Country code>-\<Mobile phone number> format.
+        # 
+        # > Mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are not supported.
         self.secure_mobile_phone = secure_mobile_phone
+        # The verification code.
+        # 
+        # You can call the [SendVerificationCodeForBindSecureMobilePhone](~~SendVerificationCodeForBindSecureMobilePhone~~) operation to obtain the verification code.
         self.verification_code = verification_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -661,14 +784,15 @@
 
 
 class BindSecureMobilePhoneResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -732,14 +856,15 @@
 
 
 class CancelChangeAccountEmailRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -759,14 +884,15 @@
 
 
 class CancelChangeAccountEmailResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -830,14 +956,15 @@
 
 
 class CancelHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
+        # The ID of the invitation.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -867,24 +994,44 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The description of the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -945,15 +1092,17 @@
 
 class CancelHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: CancelHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
+        # The information of the invitation.
         self.handshake = handshake
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -1025,16 +1174,21 @@
 class CancelMessageContactUpdateRequest(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         email_address: str = None,
         phone_number: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The email address of the contact.
         self.email_address = email_address
+        # The mobile phone number of the contact.
+        # 
+        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
         self.phone_number = phone_number
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1062,14 +1216,15 @@
 
 
 class CancelMessageContactUpdateResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1134,15 +1289,19 @@
 
 class ChangeAccountEmailRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         email: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The email address to be bound to the member.
+        # 
+        # > The system automatically sends a verification email to the email address. After the verification is passed, the email address takes effect, and the system changes both the logon email address and secure email address of the member.
         self.email = email
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1166,14 +1325,15 @@
 
 
 class ChangeAccountEmailResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1237,14 +1397,15 @@
 
 
 class CheckAccountDeleteRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1264,14 +1425,15 @@
 
 
 class CheckAccountDeleteResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1338,17 +1500,33 @@
     def __init__(
         self,
         description: str = None,
         effect_scope: str = None,
         policy_document: str = None,
         policy_name: str = None,
     ):
+        # The description of the access control policy.
+        # 
+        # The description must be 1 to 1,024 characters in length. The description can contain letters, digits, underscores (\_), and hyphens (-) and must start with a letter.
         self.description = description
+        # The effective scope of the access control policy.
+        # 
+        # The value RAM indicates that the access control policy takes effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
+        # The document of the access control policy.
+        # 
+        # The document can be a maximum of 4,096 characters in length.
+        # 
+        # For more information about the languages of access control policies, see [Languages of access control policies](~~179096~~).
+        # 
+        # For more information about the examples of access control policies, see [Examples of custom access control policies](~~181474~~).
         self.policy_document = policy_document
+        # The name of the access control policy.
+        # 
+        # The name must be 1 to 128 characters in length. The name can contain letters, digits, and hyphens (-) and must start with a letter.
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1387,21 +1565,34 @@
         description: str = None,
         effect_scope: str = None,
         policy_id: str = None,
         policy_name: str = None,
         policy_type: str = None,
         update_date: str = None,
     ):
+        # The number of times that the access control policy is referenced.
         self.attachment_count = attachment_count
+        # The time when the access control policy was created.
         self.create_date = create_date
+        # The description of the access control policy.
         self.description = description
+        # The effective scope of the access control policy.
+        # 
+        # The value RAM indicates that the access control policy takes effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The name of the access control policy.
         self.policy_name = policy_name
+        # The type of the access control policy. Valid values:
+        # 
+        # *   System: system access control policy
+        # *   Custom: custom access control policy
         self.policy_type = policy_type
+        # The time when the access control policy was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1450,15 +1641,17 @@
 
 class CreateControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         control_policy: CreateControlPolicyResponseBodyControlPolicy = None,
         request_id: str = None,
     ):
+        # The details of the access control policy.
         self.control_policy = control_policy
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.control_policy:
             self.control_policy.validate()
 
     def to_map(self):
@@ -1529,15 +1722,19 @@
 
 class CreateFolderRequest(TeaModel):
     def __init__(
         self,
         folder_name: str = None,
         parent_folder_id: str = None,
     ):
+        # The name of the folder.
+        # 
+        # The name must be 1 to 24 characters in length and can contain letters, digits, underscores (\_), periods (.),and hyphens (-).
         self.folder_name = folder_name
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1564,17 +1761,21 @@
     def __init__(
         self,
         create_time: str = None,
         folder_id: str = None,
         folder_name: str = None,
         parent_folder_id: str = None,
     ):
+        # The time when the folder was created.
         self.create_time = create_time
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The name of the folder.
         self.folder_name = folder_name
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1607,15 +1808,17 @@
 
 class CreateFolderResponseBody(TeaModel):
     def __init__(
         self,
         folder: CreateFolderResponseBodyFolder = None,
         request_id: str = None,
     ):
+        # The information about the folder.
         self.folder = folder
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.folder:
             self.folder.validate()
 
     def to_map(self):
@@ -1686,15 +1889,17 @@
 
 class CreateResourceAccountRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # The key of the tag.
         self.key = key
+        # The value of the tag.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1723,19 +1928,44 @@
         account_name_prefix: str = None,
         display_name: str = None,
         parent_folder_id: str = None,
         payer_account_id: str = None,
         resell_account_type: str = None,
         tag: List[CreateResourceAccountRequestTag] = None,
     ):
+        # The prefix for the Alibaba Cloud account name of the member. If you leave this parameter empty, the system randomly generates a prefix.
+        # 
+        # The prefix must be 2 to 37 characters in length.
+        # 
+        # The prefix can contain letters, digits, and special characters but cannot contain consecutive special characters. The prefix must start with a letter or digit and end with a letter or digit. Valid special characters include underscores (`_`), periods (.), and hyphens (`-`).
+        # 
+        # The complete Alibaba Cloud account name of a member in a resource directory is in the @.aliyunid.com format, such as `alice@rd-3G****.aliyunid.com`.
+        # 
+        # Each name must be unique in the resource directory.
         self.account_name_prefix = account_name_prefix
+        # The display name of the member.
+        # 
+        # The name must be 2 to 50 characters in length.
+        # 
+        # The name can contain letters, digits, underscores (\_), periods (.), hyphens (-), and spaces.
+        # 
+        # The name must be unique in the resource directory.
         self.display_name = display_name
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
+        # The ID of the billing account. If you leave this parameter empty, the member is used as its own billing account.
         self.payer_account_id = payer_account_id
+        # The identity type of the member. Valid values:
+        # 
+        # *   resell: The member is an account for a reseller. This is the default value. A relationship is automatically established between the member and the reseller. The management account of the resource directory must be used as the billing account of the member.
+        # *   non_resell: The member is not an account for a reseller. The member is an account that is not associated with a reseller. You can directly use the account to purchase Alibaba Cloud resources. The member is used as its own billing account.
+        # 
+        # > This parameter is available only for resellers at the international site (alibabacloud.com).
         self.resell_account_type = resell_account_type
+        # The tag of the member.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -1792,23 +2022,36 @@
         join_method: str = None,
         join_time: str = None,
         modify_time: str = None,
         resource_directory_id: str = None,
         status: str = None,
         type: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The Alibaba Cloud account name of the member.
         self.account_name = account_name
+        # The display name of the member.
         self.display_name = display_name
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time
+        # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the member. The value CreateSuccess indicates that the member is created.
         self.status = status
+        # The type of the member. The value ResourceAccount indicates that the member is a resource account.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1865,15 +2108,17 @@
 
 class CreateResourceAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: CreateResourceAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
+        # The information of the member.
         self.account = account
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -1943,14 +2188,15 @@
 
 
 class DeclineHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
+        # The ID of the invitation.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1980,24 +2226,44 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created.
         self.create_time = create_time
+        # The time when the invitation expires.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The time when the invitation was modified.
         self.modify_time = modify_time
+        # The description of the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2058,15 +2324,17 @@
 
 class DeclineHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: DeclineHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
+        # The information of the invitation.
         self.handshake = handshake
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -2137,15 +2405,19 @@
 
 class DeleteAccountRequest(TeaModel):
     def __init__(
         self,
         abandonable_check_id: List[str] = None,
         account_id: str = None,
     ):
+        # The IDs of the check items that you can choose to ignore for the member deletion.
+        # 
+        # You can obtain the IDs from the response of the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation.
         self.abandonable_check_id = abandonable_check_id
+        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2170,15 +2442,19 @@
 
 class DeleteAccountShrinkRequest(TeaModel):
     def __init__(
         self,
         abandonable_check_id_shrink: str = None,
         account_id: str = None,
     ):
+        # The IDs of the check items that you can choose to ignore for the member deletion.
+        # 
+        # You can obtain the IDs from the response of the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation.
         self.abandonable_check_id_shrink = abandonable_check_id_shrink
+        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2203,15 +2479,20 @@
 
 class DeleteAccountResponseBody(TeaModel):
     def __init__(
         self,
         deletion_type: str = None,
         request_id: str = None,
     ):
+        # The type of the deletion. Valid values:
+        # 
+        # *   0: direct deletion. If the member does not have pay-as-you-go resources that are purchased within the previous 30 days, the system directly deletes the member.
+        # *   1: deletion with a silence period. If the member has pay-as-you-go resources that are purchased within the previous 30 days, the member enters a silence period of 45 days. The system starts to delete the member until the silence period ends. For more information about the silence period, see [What is the silence period for member deletion?](~~446079~~)
         self.deletion_type = deletion_type
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2279,14 +2560,15 @@
 
 
 class DeleteControlPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
     ):
+        # The ID of the access control policy.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2306,14 +2588,15 @@
 
 
 class DeleteControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2377,14 +2660,15 @@
 
 
 class DeleteFolderRequest(TeaModel):
     def __init__(
         self,
         folder_id: str = None,
     ):
+        # The ID of the folder.
         self.folder_id = folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2404,14 +2688,15 @@
 
 
 class DeleteFolderResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2476,15 +2761,20 @@
 
 class DeleteMessageContactRequest(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         retain_contact_in_members: bool = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # Specifies whether to retain the contact for members. Valid values:
+        # 
+        # *   true (default): retains the contact for members. In this case, the contact can still receive messages for the members.
+        # *   false: does not retain the contact for members. In this case, the contact can no longer receive messages for the members. If you set this parameter to false, the response is asynchronously returned. You can call [GetMessageContactDeletionStatus](~~GetMessageContactDeletionStatus~~) to obtain the deletion result.
         self.retain_contact_in_members = retain_contact_in_members
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2509,15 +2799,20 @@
 
 class DeleteMessageContactResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         status: str = None,
     ):
+        # The request ID.
         self.request_id = request_id
+        # The deletion status of the contact. Valid values:
+        # 
+        # *   Deleting
+        # *   Deleted
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2586,15 +2881,17 @@
 
 class DeregisterDelegatedAdministratorRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         service_principal: str = None,
     ):
+        # The Alibaba Cloud account ID of the member in the resource directory.
         self.account_id = account_id
+        # The identifier of the trusted service.
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2618,14 +2915,15 @@
 
 
 class DeregisterDelegatedAdministratorResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2761,15 +3059,21 @@
 
 class DetachControlPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
         target_id: str = None,
     ):
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The ID of the object from which you want to detach the access control policy. Access control policies can be attached to the following objects:
+        # 
+        # *   Root folder
+        # *   Subfolders of the Root folder
+        # *   Members
         self.target_id = target_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2793,14 +3097,15 @@
 
 
 class DetachControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2942,15 +3247,17 @@
 
 class DisassociateMembersRequest(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         members: List[str] = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The IDs of objects from which you want to unbind the contact.
         self.members = members
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2976,16 +3283,23 @@
 class DisassociateMembersResponseBodyMembers(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         member_id: str = None,
         modify_date: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The ID of the object. Valid values:
+        # 
+        # - ID of the resource directory
+        # - ID of the folder
+        # - ID of the member
         self.member_id = member_id
+        # The time when the contact was unbound from the object.
         self.modify_date = modify_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3014,15 +3328,17 @@
 
 class DisassociateMembersResponseBody(TeaModel):
     def __init__(
         self,
         members: List[DisassociateMembersResponseBodyMembers] = None,
         request_id: str = None,
     ):
+        # The time when the contact was unbound from the object.
         self.members = members
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.members:
             for k in self.members:
                 if k:
                     k.validate()
@@ -3178,17 +3494,34 @@
     def __init__(
         self,
         enable_mode: str = None,
         maname: str = None,
         masecure_mobile_phone: str = None,
         verification_code: str = None,
     ):
+        # The mode in which you enable a resource directory. Valid values:
+        # 
+        # *   CurrentAccount: The current account is used to enable a resource directory.
+        # *   NewManagementAccount: A newly created account is used to enable a resource directory. If you select this mode, you must configure the `MAName`, `MASecureMobilePhone`, and `VerificationCode` parameters.
         self.enable_mode = enable_mode
+        # The name of the newly created account.
+        # 
+        # Specify the name in the `<Prefix>@rdadmin.aliyunid.com` format. The prefix can contain letters, digits, and special characters but cannot contain consecutive special characters. The prefix must start and end with a letter or digit. Valid special characters include underscores (`_`), periods (.), and hyphens (-). The prefix must be 2 to 50 characters in length.
         self.maname = maname
+        # The mobile phone number that is bound to the newly created account.
+        # 
+        # If you leave this parameter empty, the mobile phone number that is bound to the current account is used. The mobile phone number you specify must be the same as the mobile phone number that you specify when you call the [SendVerificationCodeForEnableRD](~~SendVerificationCodeForEnableRD~~) operation to obtain a verification code.
+        # 
+        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
+        # 
+        # > Mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are not supported.
         self.masecure_mobile_phone = masecure_mobile_phone
+        # The verification code.
+        # 
+        # You can call the [SendVerificationCodeForEnableRD](~~SendVerificationCodeForEnableRD~~) operation to obtain the verification code.
         self.verification_code = verification_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3224,18 +3557,23 @@
         self,
         create_time: str = None,
         master_account_id: str = None,
         master_account_name: str = None,
         resource_directory_id: str = None,
         root_folder_id: str = None,
     ):
+        # The time when the resource directory was enabled.
         self.create_time = create_time
+        # The ID of the management account.
         self.master_account_id = master_account_id
+        # The name of the management account.
         self.master_account_name = master_account_name
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The ID of the Root folder.
         self.root_folder_id = root_folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3272,15 +3610,17 @@
 
 class EnableResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         resource_directory: EnableResourceDirectoryResponseBodyResourceDirectory = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
+        # The information about the resource directory.
         self.resource_directory = resource_directory
 
     def validate(self):
         if self.resource_directory:
             self.resource_directory.validate()
 
     def to_map(self):
@@ -3351,15 +3691,20 @@
 
 class GetAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         include_tags: bool = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # Specifies whether to return the information of tags. Valid values:
+        # 
+        # *   false (default value)
+        # *   true
         self.include_tags = include_tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3384,15 +3729,17 @@
 
 class GetAccountResponseBodyAccountTags(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # A tag key.
         self.key = key
+        # A tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3430,28 +3777,62 @@
         modify_time: str = None,
         resource_directory_id: str = None,
         resource_directory_path: str = None,
         status: str = None,
         tags: List[GetAccountResponseBodyAccountTags] = None,
         type: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The Alibaba Cloud account name of the member.
         self.account_name = account_name
+        # The display name of the member.
         self.display_name = display_name
+        # The status of the modification for the email address bound to the member. Valid values:
+        # 
+        # *   If the value of this parameter is empty, no modification is performed for the email address.
+        # *   WAIT_MODIFY: The modification is being performed.
+        # *   CANCELLED: The modification is canceled.
+        # *   EXPIRED: The modification expires.
         self.email_status = email_status
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The real-name verification information.
         self.identity_information = identity_information
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member joined the resource directory.
         self.join_time = join_time
+        # The location of the member in the resource directory.
         self.location = location
+        # The time when the member was modified.
         self.modify_time = modify_time
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The path of the member in the resource directory.
         self.resource_directory_path = resource_directory_path
+        # The status of the member. Valid values:
+        # 
+        # *   CreateSuccess: The member is created.
+        # *   PromoteVerifying: The upgrade of the member is being confirmed.
+        # *   PromoteFailed: The upgrade of the member fails.
+        # *   PromoteExpired: The upgrade of the member expires.
+        # *   PromoteCancelled: The upgrade of the member is canceled.
+        # *   PromoteSuccess: The member is upgraded.
+        # *   InviteSuccess: The member accepts the invitation.
         self.status = status
+        # The tags of the member.
         self.tags = tags
+        # The type of the member. Valid values:
+        # 
+        # *   CloudAccount: cloud account
+        # *   ResourceAccount: resource account
         self.type = type
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -3536,15 +3917,17 @@
 
 class GetAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: GetAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
+        # The information of the member.
         self.account = account
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -3614,14 +3997,15 @@
 
 
 class GetAccountDeletionCheckResultRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3643,16 +4027,19 @@
 class GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoAbandonableChecks(TeaModel):
     def __init__(
         self,
         check_id: str = None,
         check_name: str = None,
         description: str = None,
     ):
+        # The ID of the check item.
         self.check_id = check_id
+        # The name of the cloud service to which the check item belongs.
         self.check_name = check_name
+        # The description of the check item.
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3682,16 +4069,19 @@
 class GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoNotAllowReason(TeaModel):
     def __init__(
         self,
         check_id: str = None,
         check_name: str = None,
         description: str = None,
     ):
+        # The ID of the check item.
         self.check_id = check_id
+        # The name of the cloud service to which the check item belongs.
         self.check_name = check_name
+        # The description of the check item.
         self.description = description
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3722,17 +4112,31 @@
     def __init__(
         self,
         abandonable_checks: List[GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoAbandonableChecks] = None,
         allow_delete: str = None,
         not_allow_reason: List[GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoNotAllowReason] = None,
         status: str = None,
     ):
+        # The check items that you can choose to ignore for the member deletion.
+        # 
+        # > This parameter may be returned if the value of AllowDelete is true.
         self.abandonable_checks = abandonable_checks
+        # Indicates whether the member can be deleted. Valid values:
+        # 
+        # *   true: The member can be deleted.
+        # *   false: The member cannot be deleted.
         self.allow_delete = allow_delete
+        # The reasons why the member cannot be deleted.
+        # 
+        # > This parameter is returned only if the value of AllowDelete is false.
         self.not_allow_reason = not_allow_reason
+        # The status of the check. Valid values:
+        # 
+        # *   PreCheckComplete: The check is complete.
+        # *   PreChecking: The check is in progress.
         self.status = status
 
     def validate(self):
         if self.abandonable_checks:
             for k in self.abandonable_checks:
                 if k:
                     k.validate()
@@ -3782,15 +4186,17 @@
 
 class GetAccountDeletionCheckResultResponseBody(TeaModel):
     def __init__(
         self,
         account_deletion_check_result_info: GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfo = None,
         request_id: str = None,
     ):
+        # The result of the deletion check for the member.
         self.account_deletion_check_result_info = account_deletion_check_result_info
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account_deletion_check_result_info:
             self.account_deletion_check_result_info.validate()
 
     def to_map(self):
@@ -3860,14 +4266,15 @@
 
 
 class GetAccountDeletionStatusRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3888,15 +4295,17 @@
 
 class GetAccountDeletionStatusResponseBodyRdAccountDeletionStatusFailReasonList(TeaModel):
     def __init__(
         self,
         description: str = None,
         name: str = None,
     ):
+        # The description of the check item.
         self.description = description
+        # The name of the cloud service to which the check item belongs.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3925,19 +4334,34 @@
         account_id: str = None,
         create_time: str = None,
         deletion_time: str = None,
         deletion_type: str = None,
         fail_reason_list: List[GetAccountDeletionStatusResponseBodyRdAccountDeletionStatusFailReasonList] = None,
         status: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The start time of the deletion.
         self.create_time = create_time
+        # The end time of the deletion.
         self.deletion_time = deletion_time
+        # The type of the deletion. Valid values:
+        # 
+        # *   0: direct deletion. If the member does not have pay-as-you-go resources that are purchased within the previous 30 days, the system directly deletes the member.
+        # *   1: deletion with a silence period. If the member has pay-as-you-go resources that are purchased within the previous 30 days, the member enters a silence period of 45 days. The system starts to delete the member until the silence period ends. For more information about the silence period, see [What is the silence period for member deletion?](~~446079~~)
         self.deletion_type = deletion_type
+        # The reasons why the member fails to be deleted.
         self.fail_reason_list = fail_reason_list
+        # The status. Valid values:
+        # 
+        # *   Success: The member is deleted.
+        # *   Checking: A deletion check is being performed for the member.
+        # *   Deleting: The member is being deleted.
+        # *   CheckFailed: The deletion check for the member fails.
+        # *   DeleteFailed: The member fails to be deleted.
         self.status = status
 
     def validate(self):
         if self.fail_reason_list:
             for k in self.fail_reason_list:
                 if k:
                     k.validate()
@@ -3986,15 +4410,17 @@
 
 class GetAccountDeletionStatusResponseBody(TeaModel):
     def __init__(
         self,
         rd_account_deletion_status: GetAccountDeletionStatusResponseBodyRdAccountDeletionStatus = None,
         request_id: str = None,
     ):
+        # The deletion status of the member.
         self.rd_account_deletion_status = rd_account_deletion_status
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.rd_account_deletion_status:
             self.rd_account_deletion_status.validate()
 
     def to_map(self):
@@ -4065,15 +4491,23 @@
 
 class GetControlPolicyRequest(TeaModel):
     def __init__(
         self,
         language: str = None,
         policy_id: str = None,
     ):
+        # The language in which you want to return the description of the access control policy. Valid values:
+        # 
+        # *   zh-CN (default value): Chinese
+        # *   en: English
+        # *   ja: Japanese
+        # 
+        # > This parameter is valid only for system access control policies.
         self.language = language
+        # The ID of the access control policy.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4105,22 +4539,37 @@
         effect_scope: str = None,
         policy_document: str = None,
         policy_id: str = None,
         policy_name: str = None,
         policy_type: str = None,
         update_date: str = None,
     ):
+        # The number of times that the access control policy is referenced.
         self.attachment_count = attachment_count
+        # The time when the access control policy was created.
         self.create_date = create_date
+        # The description of the access control policy.
         self.description = description
+        # The effective scope of the access control policy. Valid values:
+        # 
+        # *   All: The access control policy is in effect for Alibaba Cloud accounts, RAM users, and RAM roles.
+        # *   RAM: The access control policy is in effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope
+        # The document of the access control policy.
         self.policy_document = policy_document
+        # The ID of the access control policy.
         self.policy_id = policy_id
+        # The name of the access control policy.
         self.policy_name = policy_name
+        # The type of the access control policy. Valid values:
+        # 
+        # *   System: system access control policy
+        # *   Custom: custom access control policy
         self.policy_type = policy_type
+        # The time when the access control policy was updated.
         self.update_date = update_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4173,15 +4622,17 @@
 
 class GetControlPolicyResponseBody(TeaModel):
     def __init__(
         self,
         control_policy: GetControlPolicyResponseBodyControlPolicy = None,
         request_id: str = None,
     ):
+        # The details of the access control policy.
         self.control_policy = control_policy
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.control_policy:
             self.control_policy.validate()
 
     def to_map(self):
@@ -4328,14 +4779,15 @@
 
 
 class GetFolderRequest(TeaModel):
     def __init__(
         self,
         folder_id: str = None,
     ):
+        # The ID of the folder.
         self.folder_id = folder_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4359,18 +4811,23 @@
         self,
         create_time: str = None,
         folder_id: str = None,
         folder_name: str = None,
         parent_folder_id: str = None,
         resource_directory_path: str = None,
     ):
+        # The time when the folder was created.
         self.create_time = create_time
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The name of the folder.
         self.folder_name = folder_name
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
+        # The path of the folder in the resource directory.
         self.resource_directory_path = resource_directory_path
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4407,15 +4864,17 @@
 
 class GetFolderResponseBody(TeaModel):
     def __init__(
         self,
         folder: GetFolderResponseBodyFolder = None,
         request_id: str = None,
     ):
+        # The information about the folder.
         self.folder = folder
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.folder:
             self.folder.validate()
 
     def to_map(self):
@@ -4485,14 +4944,15 @@
 
 
 class GetHandshakeRequest(TeaModel):
     def __init__(
         self,
         handshake_id: str = None,
     ):
+        # The ID of the invitation.
         self.handshake_id = handshake_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4524,26 +4984,52 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The real-name verification information of the invitee.
+        # 
+        # > This parameter is available only when an invitee calls this operation.
         self.invited_account_real_name = invited_account_real_name
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The real-name verification information of the management account of the resource directory.
+        # 
+        # > This parameter is available only when an invitee calls this operation.
         self.master_account_real_name = master_account_real_name
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The description of the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4612,15 +5098,17 @@
 
 class GetHandshakeResponseBody(TeaModel):
     def __init__(
         self,
         handshake: GetHandshakeResponseBodyHandshake = None,
         request_id: str = None,
     ):
+        # The information of the invitation.
         self.handshake = handshake
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -4690,14 +5178,15 @@
 
 
 class GetMessageContactRequest(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4725,22 +5214,35 @@
         members: List[str] = None,
         message_types: List[str] = None,
         name: str = None,
         phone_number: str = None,
         status: str = None,
         title: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The time when the contact was created.
         self.create_date = create_date
+        # The email address of the contact.
         self.email_address = email_address
+        # The IDs of objects to which the contact is bound.
         self.members = members
+        # The types of messages received by the contact.
         self.message_types = message_types
+        # The name of the contact.
         self.name = name
+        # The mobile phone number of the contact.
         self.phone_number = phone_number
+        # The status of the contact. Valid values:
+        # 
+        # *   Verifying
+        # *   Active
+        # *   Deleting
         self.status = status
+        # The job title of the contact.
         self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4793,15 +5295,17 @@
 
 class GetMessageContactResponseBody(TeaModel):
     def __init__(
         self,
         contact: GetMessageContactResponseBodyContact = None,
         request_id: str = None,
     ):
+        # The information about the contact.
         self.contact = contact
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.contact:
             self.contact.validate()
 
     def to_map(self):
@@ -4871,14 +5375,15 @@
 
 
 class GetMessageContactDeletionStatusRequest(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4899,15 +5404,17 @@
 
 class GetMessageContactDeletionStatusResponseBodyContactDeletionStatusFailReasonList(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         message_types: List[str] = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The types of messages received by the contact.
         self.message_types = message_types
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4933,16 +5440,22 @@
 class GetMessageContactDeletionStatusResponseBodyContactDeletionStatus(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         fail_reason_list: List[GetMessageContactDeletionStatusResponseBodyContactDeletionStatusFailReasonList] = None,
         status: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The types of messages received by the contact.
         self.fail_reason_list = fail_reason_list
+        # The deletion status of the contact. Valid values:
+        # 
+        # *   Deleting
+        # *   Failed
         self.status = status
 
     def validate(self):
         if self.fail_reason_list:
             for k in self.fail_reason_list:
                 if k:
                     k.validate()
@@ -4979,15 +5492,17 @@
 
 class GetMessageContactDeletionStatusResponseBody(TeaModel):
     def __init__(
         self,
         contact_deletion_status: GetMessageContactDeletionStatusResponseBodyContactDeletionStatus = None,
         request_id: str = None,
     ):
+        # The deletion information of the contact.
         self.contact_deletion_status = contact_deletion_status
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.contact_deletion_status:
             self.contact_deletion_status.validate()
 
     def to_map(self):
@@ -5320,15 +5835,17 @@
 
 class InviteAccountToResourceDirectoryRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
+        # The tag key.
         self.key = key
+        # The tag value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5356,18 +5873,28 @@
         self,
         note: str = None,
         parent_folder_id: str = None,
         tag: List[InviteAccountToResourceDirectoryRequestTag] = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The description of the invitation.
+        # 
+        # The description can be up to 1,024 characters in length.
         self.note = note
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id
+        # The tag value.
         self.tag = tag
+        # The ID or logon email address of the account that you want to invite.
         self.target_entity = target_entity
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -5421,24 +5948,44 @@
         modify_time: str = None,
         note: str = None,
         resource_directory_id: str = None,
         status: str = None,
         target_entity: str = None,
         target_type: str = None,
     ):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time
+        # The ID of the invitation.
         self.handshake_id = handshake_id
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The description of the invitation.
         self.note = note
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending
+        # *   Accepted
+        # *   Cancelled
+        # *   Declined
+        # *   Expired
         self.status = status
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5499,15 +6046,17 @@
 
 class InviteAccountToResourceDirectoryResponseBody(TeaModel):
     def __init__(
         self,
         handshake: InviteAccountToResourceDirectoryResponseBodyHandshake = None,
         request_id: str = None,
     ):
+        # The information about the invitation.
         self.handshake = handshake
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -8384,16 +8933,19 @@
 class ListMessageContactVerificationsRequest(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The page number.
         self.page_number = page_number
+        # The number of entries per page.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8422,15 +8974,20 @@
 
 class ListMessageContactVerificationsResponseBodyContactVerifications(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         target: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The object that is used for verification. Valid values:
+        # 
+        # - Mobile phone number
+        # - Email address
         self.target = target
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8458,18 +9015,23 @@
         self,
         contact_verifications: List[ListMessageContactVerificationsResponseBodyContactVerifications] = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The record for the contact to be verified.
         self.contact_verifications = contact_verifications
+        # The page number.
         self.page_number = page_number
+        # The number of entries per page.
         self.page_size = page_size
+        # The request ID.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.contact_verifications:
             for k in self.contact_verifications:
                 if k:
                     k.validate()
@@ -8560,17 +9122,25 @@
     def __init__(
         self,
         contact_id: str = None,
         member: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The ID of the object to which the contact is bound. Valid values:
+        # 
+        # *   ID of the resource directory
+        # *   ID of the folder
+        # *   ID of the member
         self.member = member
+        # The page number.
         self.page_number = page_number
+        # The number of entries per page.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8611,23 +9181,37 @@
         members: List[str] = None,
         message_types: List[str] = None,
         name: str = None,
         phone_number: str = None,
         status: str = None,
         title: str = None,
     ):
+        # The time when the contact was bound to the objects.
         self.associated_date = associated_date
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The time when the contact was added.
         self.create_date = create_date
+        # The email address of the contact.
         self.email_address = email_address
+        # The IDs of objects to which the contact is bound.
         self.members = members
+        # The types of messages received by the contact.
         self.message_types = message_types
+        # The name of the contact.
         self.name = name
+        # The mobile phone number of the contact.
         self.phone_number = phone_number
+        # The status of the contact. Valid values:
+        # 
+        # - Verifying
+        # - Active
+        # - Deleting
         self.status = status
+        # The job title of the contact.
         self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8687,18 +9271,23 @@
         self,
         contacts: List[ListMessageContactsResponseBodyContacts] = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The time when the contact was bound to the objects.
         self.contacts = contacts
+        # The page number.
         self.page_number = page_number
+        # The number of entries per page.
         self.page_size = page_size
+        # The request ID.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.contacts:
             for k in self.contacts:
                 if k:
                     k.validate()
@@ -9279,16 +9868,28 @@
 class ListTrustedServiceStatusRequest(TeaModel):
     def __init__(
         self,
         admin_account_id: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
+        # The ID of the management account or delegated administrator account.
+        # 
+        # *   If you set this parameter to the ID of a management account, the trusted services that are enabled within the management account are queried. The default value of this parameter is the ID of an management account.
+        # *   If you set this parameter to the ID of a delegated administrator account, the trusted services that are enabled within the delegated administrator account are queried.
+        # 
+        # For more information about trusted services and delegated administrator accounts, see [Overview of trusted services](~~208133~~) and [Delegated administrator accounts](~~208117~~).
         self.admin_account_id = admin_account_id
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9317,15 +9918,17 @@
 
 class ListTrustedServiceStatusResponseBodyEnabledServicePrincipalsEnabledServicePrincipal(TeaModel):
     def __init__(
         self,
         enable_time: str = None,
         service_principal: str = None,
     ):
+        # The time when the trusted service was enabled.
         self.enable_time = enable_time
+        # The identifier of the trusted service.
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9388,18 +9991,23 @@
         self,
         enabled_service_principals: ListTrustedServiceStatusResponseBodyEnabledServicePrincipals = None,
         page_number: int = None,
         page_size: int = None,
         request_id: str = None,
         total_count: int = None,
     ):
+        # The information about the trusted services that are enabled.
         self.enabled_service_principals = enabled_service_principals
+        # The page number of the returned page.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The ID of the request.
         self.request_id = request_id
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.enabled_service_principals:
             self.enabled_service_principals.validate()
 
     def to_map(self):
@@ -9589,15 +10197,19 @@
 
 class RegisterDelegatedAdministratorRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         service_principal: str = None,
     ):
+        # The Alibaba Cloud account ID of the member in the resource directory.
         self.account_id = account_id
+        # The identifier of the trusted service.
+        # 
+        # For more information, see the `Trusted service identifier` column in [Supported trusted services](~~208133~~).
         self.service_principal = service_principal
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9621,14 +10233,15 @@
 
 
 class RegisterDelegatedAdministratorResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9893,15 +10506,19 @@
 
 class SendEmailVerificationForMessageContactRequest(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         email_address: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The email address of the contact.
+        # 
+        # The specified email address must be the one you specify when you call [AddMessageContact](~~AddMessageContact~~).
         self.email_address = email_address
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9925,14 +10542,15 @@
 
 
 class SendEmailVerificationForMessageContactResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9997,15 +10615,21 @@
 
 class SendPhoneVerificationForMessageContactRequest(TeaModel):
     def __init__(
         self,
         contact_id: str = None,
         phone_number: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The mobile phone number of the contact.
+        # 
+        # The value must be in the `<Country code>-<Mobile phone number>` format.
+        # 
+        # The specified mobile phone number must be the one you specify when you call the [AddMessageContact](~~AddMessageContact~~) operation.
         self.phone_number = phone_number
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10029,14 +10653,15 @@
 
 
 class SendPhoneVerificationForMessageContactResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10750,16 +11375,26 @@
 class UpdateAccountRequest(TeaModel):
     def __init__(
         self,
         account_id: str = None,
         new_account_type: str = None,
         new_display_name: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The new type of the member. Valid values:
+        # 
+        # *   ResourceAccount: resource account
+        # *   CloudAccount: cloud account
+        # 
+        # > You can specify either `NewDisplayName` or `NewAccountType`.
         self.new_account_type = new_account_type
+        # The new display name of the member.
+        # 
+        # > You can specify either `NewDisplayName` or `NewAccountType`.
         self.new_display_name = new_display_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10796,23 +11431,44 @@
         join_method: str = None,
         join_time: str = None,
         modify_time: str = None,
         resource_directory_id: str = None,
         status: str = None,
         type: str = None,
     ):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id
+        # The Alibaba Cloud account name of the member.
         self.account_name = account_name
+        # The display name of the member.
         self.display_name = display_name
+        # The ID of the folder.
         self.folder_id = folder_id
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method
+        # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time
+        # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id
+        # The status of the member. Valid values:
+        # 
+        # *   CreateSuccess: The member is created.
+        # *   InviteSuccess: The member accepts the invitation.
+        # *   Removed: The member is removed.
+        # *   SwitchSuccess: The type of the member is switched.
         self.status = status
+        # The type of the member. Valid values:
+        # 
+        # *   CloudAccount: cloud account
+        # *   ResourceAccount: resource account
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10869,15 +11525,17 @@
 
 class UpdateAccountResponseBody(TeaModel):
     def __init__(
         self,
         account: UpdateAccountResponseBodyAccount = None,
         request_id: str = None,
     ):
+        # The information of the member.
         self.account = account
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -11342,19 +12000,81 @@
         contact_id: str = None,
         email_address: str = None,
         message_types: List[str] = None,
         name: str = None,
         phone_number: str = None,
         title: str = None,
     ):
+        # The ID of the contact.
         self.contact_id = contact_id
+        # The email address of the contact.
+        # 
+        # After you specify an email address, you need to call [SendEmailVerificationForMessageContact](~~SendEmailVerificationForMessageContact~~) to send verification information to the email address. After the verification is passed, the email address takes effect.
         self.email_address = email_address
+        # The types of messages received by the contact.
         self.message_types = message_types
+        # The name of the contact.
         self.name = name
+        # The mobile phone number of the contact.
+        # 
+        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
+        # 
+        # After you specify a mobile phone number, you need to call [SendPhoneVerificationForMessageContact](~~SendPhoneVerificationForMessageContact~~) to send verification information to the mobile phone number. After the verification is passed, the mobile phone number takes effect.
         self.phone_number = phone_number
+        # The job title of the contact.
+        # 
+        # Valid values:
+        # 
+        # *   FinanceDirector
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   TechnicalDirector
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   MaintenanceDirector
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   CEO
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   ProjectDirector
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        # *   Other
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
+        # 
+        #     <!-- -->
         self.title = title
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11394,14 +12114,15 @@
 
 
 class UpdateMessageContactResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcedirectorymaster20220419
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.2/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt` & `alibabacloud_resourcedirectorymaster20220419-1.0.3/alibabacloud_resourcedirectorymaster20220419.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419-1.0.2/setup.py` & `alibabacloud_resourcedirectorymaster20220419-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcedirectorymaster20220419.
 
-Created on 04/05/2023
+Created on 26/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcedirectorymaster20220419"
 NAME = "alibabacloud_resourcedirectorymaster20220419" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

