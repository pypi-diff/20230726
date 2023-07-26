# Comparing `tmp/alibabacloud_resourcedirectorymaster20220419_py2-1.0.2.tar.gz` & `tmp/alibabacloud_resourcedirectorymaster20220419_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419_py2-1.0.2.tar", last modified: Thu May  4 11:31:30 2023, max compression
+gzip compressed data, was "dist/alibabacloud_resourcedirectorymaster20220419_py2-1.0.3.tar", last modified: Wed Jul 26 01:44:00 2023, max compression
```

## Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.2.tar` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2592 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1093 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1176 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88121 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419/client.py
--rw-r--r--   0 root         (0) root         (0)   372210 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2592 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3003 2023-05-04 11:31:30.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 01:44:00.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-26 01:43:59.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-26 01:43:59.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-26 01:43:59.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-07-26 01:44:00.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-07-26 01:43:59.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-07-26 01:43:59.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 01:44:00.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-26 01:43:59.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101735 2023-07-26 01:43:59.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419/client.py
+-rw-r--r--   0 root         (0) root         (0)   408539 2023-07-26 01:43:59.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 01:44:00.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-07-26 01:44:00.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-26 01:44:00.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 01:44:00.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-26 01:44:00.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-26 01:44:00.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 01:44:00.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3003 2023-07-26 01:43:59.000000 alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/LICENSE` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_resourcedirectorymaster20220419_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/README-CN.md` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/README.md` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419/client.py` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,24 @@
         if not UtilClient.empty(endpoint):
             return endpoint
         if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
             return endpoint_map.get(region_id)
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def accept_handshake_with_options(self, request, runtime):
+        """
+        After an invited Alibaba Cloud account joins a resource directory, it becomes a member of the resource directory. By default, the name of the invited Alibaba Cloud account is used as the display name of the account in the resource directory.
+        
+
+        @param request: AcceptHandshakeRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: AcceptHandshakeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.handshake_id):
             query['HandshakeId'] = request.handshake_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -51,14 +61,22 @@
         )
         return TeaCore.from_map(
             resource_directory_master_20220419_models.AcceptHandshakeResponse(),
             self.call_api(params, req, runtime)
         )
 
     def accept_handshake(self, request):
+        """
+        After an invited Alibaba Cloud account joins a resource directory, it becomes a member of the resource directory. By default, the name of the invited Alibaba Cloud account is used as the display name of the account in the resource directory.
+        
+
+        @param request: AcceptHandshakeRequest
+
+        @return: AcceptHandshakeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.accept_handshake_with_options(request, runtime)
 
     def add_message_contact_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.email_address):
@@ -122,15 +140,18 @@
 
     def associate_members(self, request):
         runtime = util_models.RuntimeOptions()
         return self.associate_members_with_options(request, runtime)
 
     def attach_control_policy_with_options(self, request, runtime):
         """
-        The ID of the request.
+        After you attach a custom access control policy, the operations performed on resources by using members are limited by the policy. Make sure that the attached policy meets your expectations. Otherwise, your business may be affected.
+        By default, the system access control policy FullAliyunAccess is attached to each folder and member.
+        The access control policy that is attached to a folder also applies to all its subfolders and all members in the subfolders.
+        A maximum of 10 access control policies can be attached to a folder or member.
         
 
         @param request: AttachControlPolicyRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: AttachControlPolicyResponse
@@ -158,27 +179,31 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.AttachControlPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     def attach_control_policy(self, request):
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
 
     def bind_secure_mobile_phone_with_options(self, request, runtime):
         """
-        The ID of the request.
+        You can call this API operation only to bind a mobile phone number to a member of the resource account type. You cannot call this API operation to change the mobile phone number that is bound to a member of the resource account type.
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this API operation.
         
 
         @param request: BindSecureMobilePhoneRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: BindSecureMobilePhoneResponse
@@ -208,15 +233,16 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.BindSecureMobilePhoneResponse(),
             self.call_api(params, req, runtime)
         )
 
     def bind_secure_mobile_phone(self, request):
         """
-        The ID of the request.
+        You can call this API operation only to bind a mobile phone number to a member of the resource account type. You cannot call this API operation to change the mobile phone number that is bound to a member of the resource account type.
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this API operation.
         
 
         @param request: BindSecureMobilePhoneRequest
 
         @return: BindSecureMobilePhoneResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -338,15 +364,15 @@
 
     def change_account_email(self, request):
         runtime = util_models.RuntimeOptions()
         return self.change_account_email_with_options(request, runtime)
 
     def check_account_delete_with_options(self, request, runtime):
         """
-        The returned result.
+        Before you delete a member, you must call this API operation to check whether the member can be deleted.
         
 
         @param request: CheckAccountDeleteRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CheckAccountDeleteResponse
@@ -372,15 +398,15 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.CheckAccountDeleteResponse(),
             self.call_api(params, req, runtime)
         )
 
     def check_account_delete(self, request):
         """
-        The returned result.
+        Before you delete a member, you must call this API operation to check whether the member can be deleted.
         
 
         @param request: CheckAccountDeleteRequest
 
         @return: CheckAccountDeleteResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -418,15 +444,15 @@
 
     def create_control_policy(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_control_policy_with_options(request, runtime)
 
     def create_folder_with_options(self, request, runtime):
         """
-        The name of the folder.
+        A maximum of five levels of folders can be created under the Root folder.
         
 
         @param request: CreateFolderRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateFolderResponse
@@ -454,27 +480,28 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.CreateFolderResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_folder(self, request):
         """
-        The name of the folder.
+        A maximum of five levels of folders can be created under the Root folder.
         
 
         @param request: CreateFolderRequest
 
         @return: CreateFolderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_folder_with_options(request, runtime)
 
     def create_resource_account_with_options(self, request, runtime):
         """
-        The Alibaba Cloud account name of the member.
+        A member serves as a container for resources and is also an organizational unit in a resource directory. A member indicates a project or application. The resources of different members are isolated.
+        This topic provides an example on how to call the API operation to create a member in the `fd-r23M55****` folder. The display name of the member is `Dev`, and the prefix for the Alibaba Cloud account name of the member is `alice`.
         
 
         @param request: CreateResourceAccountRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateResourceAccountResponse
@@ -510,15 +537,16 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.CreateResourceAccountResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_resource_account(self, request):
         """
-        The Alibaba Cloud account name of the member.
+        A member serves as a container for resources and is also an organizational unit in a resource directory. A member indicates a project or application. The resources of different members are isolated.
+        This topic provides an example on how to call the API operation to create a member in the `fd-r23M55****` folder. The display name of the member is `Dev`, and the prefix for the Alibaba Cloud account name of the member is `alice`.
         
 
         @param request: CreateResourceAccountRequest
 
         @return: CreateResourceAccountResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -549,14 +577,26 @@
         )
 
     def decline_handshake(self, request):
         runtime = util_models.RuntimeOptions()
         return self.decline_handshake_with_options(request, runtime)
 
     def delete_account_with_options(self, tmp_req, runtime):
+        """
+        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
+        Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
+        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
+        
+
+        @param tmp_req: DeleteAccountRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DeleteAccountResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = resource_directory_master_20220419_models.DeleteAccountShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.abandonable_check_id):
             request.abandonable_check_id_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.abandonable_check_id, 'AbandonableCheckId', 'json')
         query = {}
         if not UtilClient.is_unset(request.abandonable_check_id_shrink):
@@ -579,20 +619,30 @@
         )
         return TeaCore.from_map(
             resource_directory_master_20220419_models.DeleteAccountResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_account(self, request):
+        """
+        > The member deletion feature is in invitational preview. You can contact the customer business manager (CBM) of Alibaba Cloud to apply for a trial.
+        Before you delete a member, we recommend that you call the [CheckAccountDelete](~~CheckAccountDelete~~) and [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operations to check whether the member meets deletion requirements. You can call the DeleteAccount operation to delete only members that meet the deletion requirements.
+        After a member is deleted, the resources and data within the member are deleted, and you can no longer use the member to log on to the Alibaba Cloud Management Console. In addition, the member cannot be recovered. Proceed with caution. For more information about how to delete a member, see [Delete a member of the resource account type](~~446078~~).
+        
+
+        @param request: DeleteAccountRequest
+
+        @return: DeleteAccountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_account_with_options(request, runtime)
 
     def delete_control_policy_with_options(self, request, runtime):
         """
-        The ID of the request.
+        If you want to delete a custom access control policy that is attached to folders or members, you must call the [DetachControlPolicy](~~DetachControlPolicy~~) operation to detach the policy before you delete it.
         
 
         @param request: DeleteControlPolicyRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteControlPolicyResponse
@@ -618,27 +668,27 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.DeleteControlPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_control_policy(self, request):
         """
-        The ID of the request.
+        If you want to delete a custom access control policy that is attached to folders or members, you must call the [DetachControlPolicy](~~DetachControlPolicy~~) operation to detach the policy before you delete it.
         
 
         @param request: DeleteControlPolicyRequest
 
         @return: DeleteControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_control_policy_with_options(request, runtime)
 
     def delete_folder_with_options(self, request, runtime):
         """
-        The ID of the request.
+        Before you delete a folder, you must make sure that the folder does not contain members or subfolders.
         
 
         @param request: DeleteFolderRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DeleteFolderResponse
@@ -664,15 +714,15 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.DeleteFolderResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_folder(self, request):
         """
-        The ID of the request.
+        Before you delete a folder, you must make sure that the folder does not contain members or subfolders.
         
 
         @param request: DeleteFolderRequest
 
         @return: DeleteFolderResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -705,14 +755,24 @@
         )
 
     def delete_message_contact(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_message_contact_with_options(request, runtime)
 
     def deregister_delegated_administrator_with_options(self, request, runtime):
+        """
+        If the delegated administrator account that you want to remove has historical management tasks in the related trusted service, the trusted service may be affected after the delegated administrator account is removed. Therefore, proceed with caution.
+        
+
+        @param request: DeregisterDelegatedAdministratorRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DeregisterDelegatedAdministratorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.service_principal):
             query['ServicePrincipal'] = request.service_principal
         req = open_api_models.OpenApiRequest(
@@ -731,14 +791,22 @@
         )
         return TeaCore.from_map(
             resource_directory_master_20220419_models.DeregisterDelegatedAdministratorResponse(),
             self.call_api(params, req, runtime)
         )
 
     def deregister_delegated_administrator(self, request):
+        """
+        If the delegated administrator account that you want to remove has historical management tasks in the related trusted service, the trusted service may be affected after the delegated administrator account is removed. Therefore, proceed with caution.
+        
+
+        @param request: DeregisterDelegatedAdministratorRequest
+
+        @return: DeregisterDelegatedAdministratorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.deregister_delegated_administrator_with_options(request, runtime)
 
     def destroy_resource_directory_with_options(self, runtime):
         """
         The ID of the request.
         
@@ -773,14 +841,25 @@
 
         @return: DestroyResourceDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.destroy_resource_directory_with_options(runtime)
 
     def detach_control_policy_with_options(self, request, runtime):
+        """
+        After you detach an access control policy, the operations performed on resources by using members are not limited by the policy. Make sure that the detached policy meets your expectations. Otherwise, your business may be affected.
+        Both the system and custom access control policies can be detached. If an object has only one access control policy attached, the policy cannot be detached.
+        
+
+        @param request: DetachControlPolicyRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DetachControlPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.policy_id):
             query['PolicyId'] = request.policy_id
         if not UtilClient.is_unset(request.target_id):
             query['TargetId'] = request.target_id
         req = open_api_models.OpenApiRequest(
@@ -799,14 +878,23 @@
         )
         return TeaCore.from_map(
             resource_directory_master_20220419_models.DetachControlPolicyResponse(),
             self.call_api(params, req, runtime)
         )
 
     def detach_control_policy(self, request):
+        """
+        After you detach an access control policy, the operations performed on resources by using members are not limited by the policy. Make sure that the detached policy meets your expectations. Otherwise, your business may be affected.
+        Both the system and custom access control policies can be detached. If an object has only one access control policy attached, the policy cannot be detached.
+        
+
+        @param request: DetachControlPolicyRequest
+
+        @return: DetachControlPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.detach_control_policy_with_options(request, runtime)
 
     def disable_control_policy_with_options(self, runtime):
         """
         The ID of the request.
         
@@ -910,15 +998,15 @@
         @return: EnableControlPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.enable_control_policy_with_options(runtime)
 
     def enable_resource_directory_with_options(self, request, runtime):
         """
-        The ID of the request.
+        You can use the current account or a newly created account to enable a resource directory. For more information, see [Enable a resource directory](~~111215~~).
         
 
         @param request: EnableResourceDirectoryRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: EnableResourceDirectoryResponse
@@ -950,15 +1038,15 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.EnableResourceDirectoryResponse(),
             self.call_api(params, req, runtime)
         )
 
     def enable_resource_directory(self, request):
         """
-        The ID of the request.
+        You can use the current account or a newly created account to enable a resource directory. For more information, see [Enable a resource directory](~~111215~~).
         
 
         @param request: EnableResourceDirectoryRequest
 
         @return: EnableResourceDirectoryResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -992,15 +1080,15 @@
 
     def get_account(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_account_with_options(request, runtime)
 
     def get_account_deletion_check_result_with_options(self, request, runtime):
         """
-        Container Service for Kubernetes
+        After you call the [CheckAccountDelete](~~CheckAccountDelete~~) operation to perform a member deletion check, you can call the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation to query the check result. If the check result shows that the member meets deletion requirements, you can delete the member. Otherwise, you need to first modify the items that do not meet requirements.
         
 
         @param request: GetAccountDeletionCheckResultRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: GetAccountDeletionCheckResultResponse
@@ -1026,15 +1114,15 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.GetAccountDeletionCheckResultResponse(),
             self.call_api(params, req, runtime)
         )
 
     def get_account_deletion_check_result(self, request):
         """
-        Container Service for Kubernetes
+        After you call the [CheckAccountDelete](~~CheckAccountDelete~~) operation to perform a member deletion check, you can call the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation to query the check result. If the check result shows that the member meets deletion requirements, you can delete the member. Otherwise, you need to first modify the items that do not meet requirements.
         
 
         @param request: GetAccountDeletionCheckResultRequest
 
         @return: GetAccountDeletionCheckResultResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1806,15 +1894,15 @@
 
     def list_target_attachments_for_control_policy(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_target_attachments_for_control_policy_with_options(request, runtime)
 
     def list_trusted_service_status_with_options(self, request, runtime):
         """
-        The time when the trusted service was enabled.
+        Only a management account or delegated administrator account can be used to call this operation.
         
 
         @param request: ListTrustedServiceStatusRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: ListTrustedServiceStatusResponse
@@ -1844,15 +1932,15 @@
         return TeaCore.from_map(
             resource_directory_master_20220419_models.ListTrustedServiceStatusResponse(),
             self.call_api(params, req, runtime)
         )
 
     def list_trusted_service_status(self, request):
         """
-        The time when the trusted service was enabled.
+        Only a management account or delegated administrator account can be used to call this operation.
         
 
         @param request: ListTrustedServiceStatusRequest
 
         @return: ListTrustedServiceStatusResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1885,14 +1973,27 @@
         )
 
     def move_account(self, request):
         runtime = util_models.RuntimeOptions()
         return self.move_account_with_options(request, runtime)
 
     def register_delegated_administrator_with_options(self, request, runtime):
+        """
+        The delegated administrator account can be used to access the information of the resource directory and view the structure and members of the resource directory. The delegated administrator account can also be used to perform service-related management operations in the trusted service on behalf of the management account of the resource directory. When you call this operation, you must take note of the following limits:
+        *   Only some trusted services support delegated administrator accounts. For more information, see [Supported trusted services](~~208133~~).
+        *   Only the management account of a resource directory or an authorized RAM user or RAM role of the management account can be used to call this operation.
+        *   The number of delegated administrator accounts that are allowed for a trusted service is defined by the trusted service.
+        
+
+        @param request: RegisterDelegatedAdministratorRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: RegisterDelegatedAdministratorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.service_principal):
             query['ServicePrincipal'] = request.service_principal
         req = open_api_models.OpenApiRequest(
@@ -1911,14 +2012,25 @@
         )
         return TeaCore.from_map(
             resource_directory_master_20220419_models.RegisterDelegatedAdministratorResponse(),
             self.call_api(params, req, runtime)
         )
 
     def register_delegated_administrator(self, request):
+        """
+        The delegated administrator account can be used to access the information of the resource directory and view the structure and members of the resource directory. The delegated administrator account can also be used to perform service-related management operations in the trusted service on behalf of the management account of the resource directory. When you call this operation, you must take note of the following limits:
+        *   Only some trusted services support delegated administrator accounts. For more information, see [Supported trusted services](~~208133~~).
+        *   Only the management account of a resource directory or an authorized RAM user or RAM role of the management account can be used to call this operation.
+        *   The number of delegated administrator accounts that are allowed for a trusted service is defined by the trusted service.
+        
+
+        @param request: RegisterDelegatedAdministratorRequest
+
+        @return: RegisterDelegatedAdministratorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.register_delegated_administrator_with_options(request, runtime)
 
     def remove_cloud_account_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
@@ -2237,14 +2349,26 @@
         )
 
     def untag_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
 
     def update_account_with_options(self, request, runtime):
+        """
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this operation.
+        *   Before you switch the type of a member from resource account to cloud account, make sure that specific conditions are met. For more information about the conditions, see [Switch a resource account to a cloud account](~~111233~~).
+        *   Before you switch the type of a member from cloud account to resource account, make sure that specific conditions are met. For more information about the conditions, see [Switch a cloud account to a resource account](~~209980~~).
+        
+
+        @param request: UpdateAccountRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: UpdateAccountResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.new_account_type):
             query['NewAccountType'] = request.new_account_type
         if not UtilClient.is_unset(request.new_display_name):
@@ -2265,14 +2389,24 @@
         )
         return TeaCore.from_map(
             resource_directory_master_20220419_models.UpdateAccountResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_account(self, request):
+        """
+        To ensure that the system can record the operators of management operations, you must use a RAM user or RAM role to which the AliyunResourceDirectoryFullAccess policy is attached within the management account of your resource directory to call this operation.
+        *   Before you switch the type of a member from resource account to cloud account, make sure that specific conditions are met. For more information about the conditions, see [Switch a resource account to a cloud account](~~111233~~).
+        *   Before you switch the type of a member from cloud account to resource account, make sure that specific conditions are met. For more information about the conditions, see [Switch a cloud account to a resource account](~~209980~~).
+        
+
+        @param request: UpdateAccountRequest
+
+        @return: UpdateAccountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_account_with_options(request, runtime)
 
     def update_control_policy_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.new_description):
```

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419/models.py` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 
 
 class AcceptHandshakeRequest(TeaModel):
     def __init__(self, handshake_id=None):
+        # The ID of the invitation.
+        # 
+        # You can call the [ListHandshakesForAccount](~~ListHandshakesForAccount~~) operation to obtain the ID.
         self.handshake_id = handshake_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AcceptHandshakeRequest, self).to_map()
@@ -27,24 +30,44 @@
         return self
 
 
 class AcceptHandshakeResponseBodyHandshake(TeaModel):
     def __init__(self, create_time=None, expire_time=None, handshake_id=None, master_account_id=None,
                  master_account_name=None, modify_time=None, note=None, resource_directory_id=None, status=None, target_entity=None,
                  target_type=None):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time  # type: str
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time  # type: str
+        # The ID of the invitation.
         self.handshake_id = handshake_id  # type: str
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id  # type: str
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name  # type: str
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time  # type: str
+        # The description of the invitation.
         self.note = note  # type: str
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id  # type: str
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status  # type: str
+        # The ID or logon email address of the invited Alibaba Cloud account.
         self.target_entity = target_entity  # type: str
+        # The type of the invited Alibaba Cloud account. Valid values:
+        # 
+        # *   Account: indicates the ID of the Alibaba Cloud account.
+        # *   Email: indicates the logon email address of the Alibaba Cloud account.
         self.target_type = target_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AcceptHandshakeResponseBodyHandshake, self).to_map()
@@ -101,15 +124,17 @@
         if m.get('TargetType') is not None:
             self.target_type = m.get('TargetType')
         return self
 
 
 class AcceptHandshakeResponseBody(TeaModel):
     def __init__(self, handshake=None, request_id=None):
+        # The information of the invitation.
         self.handshake = handshake  # type: AcceptHandshakeResponseBodyHandshake
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -171,18 +196,83 @@
             temp_model = AcceptHandshakeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddMessageContactRequest(TeaModel):
     def __init__(self, email_address=None, message_types=None, name=None, phone_number=None, title=None):
+        # The email address of the contact.
+        # 
+        # After you specify an email address, you need to call [SendEmailVerificationForMessageContact](~~SendEmailVerificationForMessageContact~~) to send verification information to the email address. After the verification is passed, the email address takes effect.
         self.email_address = email_address  # type: str
+        # The types of messages received by the contact.
         self.message_types = message_types  # type: list[str]
+        # The name of the contact.
+        # 
+        # The name must be unique in your resource directory.
+        # 
+        # The name must be 2 to 12 characters in length and can contain only letters.
         self.name = name  # type: str
+        # The mobile phone number of the contact.
+        # 
+        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
+        # 
+        # After you specify a mobile phone number, you need to call [SendPhoneVerificationForMessageContact](~~SendPhoneVerificationForMessageContact~~) to send verification information to the mobile phone number. After the verification is passed, the mobile phone number takes effect.
         self.phone_number = phone_number  # type: str
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
         self.title = title  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AddMessageContactRequest, self).to_map()
@@ -215,15 +305,17 @@
         if m.get('Title') is not None:
             self.title = m.get('Title')
         return self
 
 
 class AddMessageContactResponseBodyContact(TeaModel):
     def __init__(self, contact_id=None, create_date=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The time when the contact was created.
         self.create_date = create_date  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AddMessageContactResponseBodyContact, self).to_map()
@@ -244,15 +336,17 @@
         if m.get('CreateDate') is not None:
             self.create_date = m.get('CreateDate')
         return self
 
 
 class AddMessageContactResponseBody(TeaModel):
     def __init__(self, contact=None, request_id=None):
+        # The information about the contact.
         self.contact = contact  # type: AddMessageContactResponseBodyContact
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.contact:
             self.contact.validate()
 
     def to_map(self):
@@ -314,15 +408,17 @@
             temp_model = AddMessageContactResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AssociateMembersRequest(TeaModel):
     def __init__(self, contact_id=None, members=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The IDs of objects to which you want to bind the contact.
         self.members = members  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AssociateMembersRequest, self).to_map()
@@ -343,16 +439,23 @@
         if m.get('Members') is not None:
             self.members = m.get('Members')
         return self
 
 
 class AssociateMembersResponseBodyMembers(TeaModel):
     def __init__(self, contact_id=None, member_id=None, modify_date=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The ID of the object. Valid values:
+        # 
+        # - ID of the resource directory
+        # - ID of the folder
+        # - ID of the member
         self.member_id = member_id  # type: str
+        # The time when the contact was bound to the object.
         self.modify_date = modify_date  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AssociateMembersResponseBodyMembers, self).to_map()
@@ -377,15 +480,17 @@
         if m.get('ModifyDate') is not None:
             self.modify_date = m.get('ModifyDate')
         return self
 
 
 class AssociateMembersResponseBody(TeaModel):
     def __init__(self, members=None, request_id=None):
+        # The time when the contact was bound to the object.
         self.members = members  # type: list[AssociateMembersResponseBodyMembers]
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.members:
             for k in self.members:
                 if k:
                     k.validate()
@@ -453,15 +558,21 @@
             temp_model = AssociateMembersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AttachControlPolicyRequest(TeaModel):
     def __init__(self, policy_id=None, target_id=None):
+        # The ID of the access control policy.
         self.policy_id = policy_id  # type: str
+        # The ID of the object to which you want to attach the access control policy. Access control policies can be attached to the following objects:
+        # 
+        # *   Root folder
+        # *   Subfolders of the Root folder
+        # *   Members
         self.target_id = target_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AttachControlPolicyRequest, self).to_map()
@@ -482,14 +593,15 @@
         if m.get('TargetId') is not None:
             self.target_id = m.get('TargetId')
         return self
 
 
 class AttachControlPolicyResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AttachControlPolicyResponseBody, self).to_map()
@@ -545,16 +657,27 @@
             temp_model = AttachControlPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BindSecureMobilePhoneRequest(TeaModel):
     def __init__(self, account_id=None, secure_mobile_phone=None, verification_code=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
+        # The mobile phone number that you want to bind to the member for security purposes.
+        # 
+        # The mobile phone number you specify must be the same as the mobile phone number that you specify when you call the [SendVerificationCodeForBindSecureMobilePhone](~~SendVerificationCodeForBindSecureMobilePhone~~) operation to obtain a verification code.
+        # 
+        # Specify the mobile phone number in the \<Country code>-\<Mobile phone number> format.
+        # 
+        # > Mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are not supported.
         self.secure_mobile_phone = secure_mobile_phone  # type: str
+        # The verification code.
+        # 
+        # You can call the [SendVerificationCodeForBindSecureMobilePhone](~~SendVerificationCodeForBindSecureMobilePhone~~) operation to obtain the verification code.
         self.verification_code = verification_code  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BindSecureMobilePhoneRequest, self).to_map()
@@ -579,14 +702,15 @@
         if m.get('VerificationCode') is not None:
             self.verification_code = m.get('VerificationCode')
         return self
 
 
 class BindSecureMobilePhoneResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(BindSecureMobilePhoneResponseBody, self).to_map()
@@ -642,14 +766,15 @@
             temp_model = BindSecureMobilePhoneResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CancelChangeAccountEmailRequest(TeaModel):
     def __init__(self, account_id=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CancelChangeAccountEmailRequest, self).to_map()
@@ -666,14 +791,15 @@
         if m.get('AccountId') is not None:
             self.account_id = m.get('AccountId')
         return self
 
 
 class CancelChangeAccountEmailResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CancelChangeAccountEmailResponseBody, self).to_map()
@@ -729,14 +855,15 @@
             temp_model = CancelChangeAccountEmailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CancelHandshakeRequest(TeaModel):
     def __init__(self, handshake_id=None):
+        # The ID of the invitation.
         self.handshake_id = handshake_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CancelHandshakeRequest, self).to_map()
@@ -755,24 +882,44 @@
         return self
 
 
 class CancelHandshakeResponseBodyHandshake(TeaModel):
     def __init__(self, create_time=None, expire_time=None, handshake_id=None, master_account_id=None,
                  master_account_name=None, modify_time=None, note=None, resource_directory_id=None, status=None, target_entity=None,
                  target_type=None):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time  # type: str
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time  # type: str
+        # The ID of the invitation.
         self.handshake_id = handshake_id  # type: str
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id  # type: str
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name  # type: str
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time  # type: str
+        # The description of the invitation.
         self.note = note  # type: str
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id  # type: str
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status  # type: str
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity  # type: str
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CancelHandshakeResponseBodyHandshake, self).to_map()
@@ -829,15 +976,17 @@
         if m.get('TargetType') is not None:
             self.target_type = m.get('TargetType')
         return self
 
 
 class CancelHandshakeResponseBody(TeaModel):
     def __init__(self, handshake=None, request_id=None):
+        # The information of the invitation.
         self.handshake = handshake  # type: CancelHandshakeResponseBodyHandshake
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -899,16 +1048,21 @@
             temp_model = CancelHandshakeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CancelMessageContactUpdateRequest(TeaModel):
     def __init__(self, contact_id=None, email_address=None, phone_number=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The email address of the contact.
         self.email_address = email_address  # type: str
+        # The mobile phone number of the contact.
+        # 
+        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
         self.phone_number = phone_number  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CancelMessageContactUpdateRequest, self).to_map()
@@ -933,14 +1087,15 @@
         if m.get('PhoneNumber') is not None:
             self.phone_number = m.get('PhoneNumber')
         return self
 
 
 class CancelMessageContactUpdateResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CancelMessageContactUpdateResponseBody, self).to_map()
@@ -996,15 +1151,19 @@
             temp_model = CancelMessageContactUpdateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ChangeAccountEmailRequest(TeaModel):
     def __init__(self, account_id=None, email=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
+        # The email address to be bound to the member.
+        # 
+        # > The system automatically sends a verification email to the email address. After the verification is passed, the email address takes effect, and the system changes both the logon email address and secure email address of the member.
         self.email = email  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ChangeAccountEmailRequest, self).to_map()
@@ -1025,14 +1184,15 @@
         if m.get('Email') is not None:
             self.email = m.get('Email')
         return self
 
 
 class ChangeAccountEmailResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ChangeAccountEmailResponseBody, self).to_map()
@@ -1088,14 +1248,15 @@
             temp_model = ChangeAccountEmailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CheckAccountDeleteRequest(TeaModel):
     def __init__(self, account_id=None):
+        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CheckAccountDeleteRequest, self).to_map()
@@ -1112,14 +1273,15 @@
         if m.get('AccountId') is not None:
             self.account_id = m.get('AccountId')
         return self
 
 
 class CheckAccountDeleteResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CheckAccountDeleteResponseBody, self).to_map()
@@ -1175,17 +1337,33 @@
             temp_model = CheckAccountDeleteResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateControlPolicyRequest(TeaModel):
     def __init__(self, description=None, effect_scope=None, policy_document=None, policy_name=None):
+        # The description of the access control policy.
+        # 
+        # The description must be 1 to 1,024 characters in length. The description can contain letters, digits, underscores (\_), and hyphens (-) and must start with a letter.
         self.description = description  # type: str
+        # The effective scope of the access control policy.
+        # 
+        # The value RAM indicates that the access control policy takes effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope  # type: str
+        # The document of the access control policy.
+        # 
+        # The document can be a maximum of 4,096 characters in length.
+        # 
+        # For more information about the languages of access control policies, see [Languages of access control policies](~~179096~~).
+        # 
+        # For more information about the examples of access control policies, see [Examples of custom access control policies](~~181474~~).
         self.policy_document = policy_document  # type: str
+        # The name of the access control policy.
+        # 
+        # The name must be 1 to 128 characters in length. The name can contain letters, digits, and hyphens (-) and must start with a letter.
         self.policy_name = policy_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateControlPolicyRequest, self).to_map()
@@ -1215,21 +1393,34 @@
             self.policy_name = m.get('PolicyName')
         return self
 
 
 class CreateControlPolicyResponseBodyControlPolicy(TeaModel):
     def __init__(self, attachment_count=None, create_date=None, description=None, effect_scope=None, policy_id=None,
                  policy_name=None, policy_type=None, update_date=None):
+        # The number of times that the access control policy is referenced.
         self.attachment_count = attachment_count  # type: str
+        # The time when the access control policy was created.
         self.create_date = create_date  # type: str
+        # The description of the access control policy.
         self.description = description  # type: str
+        # The effective scope of the access control policy.
+        # 
+        # The value RAM indicates that the access control policy takes effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope  # type: str
+        # The ID of the access control policy.
         self.policy_id = policy_id  # type: str
+        # The name of the access control policy.
         self.policy_name = policy_name  # type: str
+        # The type of the access control policy. Valid values:
+        # 
+        # *   System: system access control policy
+        # *   Custom: custom access control policy
         self.policy_type = policy_type  # type: str
+        # The time when the access control policy was updated.
         self.update_date = update_date  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateControlPolicyResponseBodyControlPolicy, self).to_map()
@@ -1274,15 +1465,17 @@
         if m.get('UpdateDate') is not None:
             self.update_date = m.get('UpdateDate')
         return self
 
 
 class CreateControlPolicyResponseBody(TeaModel):
     def __init__(self, control_policy=None, request_id=None):
+        # The details of the access control policy.
         self.control_policy = control_policy  # type: CreateControlPolicyResponseBodyControlPolicy
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.control_policy:
             self.control_policy.validate()
 
     def to_map(self):
@@ -1344,15 +1537,19 @@
             temp_model = CreateControlPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateFolderRequest(TeaModel):
     def __init__(self, folder_name=None, parent_folder_id=None):
+        # The name of the folder.
+        # 
+        # The name must be 1 to 24 characters in length and can contain letters, digits, underscores (\_), periods (.),and hyphens (-).
         self.folder_name = folder_name  # type: str
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateFolderRequest, self).to_map()
@@ -1373,17 +1570,21 @@
         if m.get('ParentFolderId') is not None:
             self.parent_folder_id = m.get('ParentFolderId')
         return self
 
 
 class CreateFolderResponseBodyFolder(TeaModel):
     def __init__(self, create_time=None, folder_id=None, folder_name=None, parent_folder_id=None):
+        # The time when the folder was created.
         self.create_time = create_time  # type: str
+        # The ID of the folder.
         self.folder_id = folder_id  # type: str
+        # The name of the folder.
         self.folder_name = folder_name  # type: str
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateFolderResponseBodyFolder, self).to_map()
@@ -1412,15 +1613,17 @@
         if m.get('ParentFolderId') is not None:
             self.parent_folder_id = m.get('ParentFolderId')
         return self
 
 
 class CreateFolderResponseBody(TeaModel):
     def __init__(self, folder=None, request_id=None):
+        # The information about the folder.
         self.folder = folder  # type: CreateFolderResponseBodyFolder
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.folder:
             self.folder.validate()
 
     def to_map(self):
@@ -1482,15 +1685,17 @@
             temp_model = CreateFolderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateResourceAccountRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
+        # The key of the tag.
         self.key = key  # type: str
+        # The value of the tag.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateResourceAccountRequestTag, self).to_map()
@@ -1512,19 +1717,44 @@
             self.value = m.get('Value')
         return self
 
 
 class CreateResourceAccountRequest(TeaModel):
     def __init__(self, account_name_prefix=None, display_name=None, parent_folder_id=None, payer_account_id=None,
                  resell_account_type=None, tag=None):
+        # The prefix for the Alibaba Cloud account name of the member. If you leave this parameter empty, the system randomly generates a prefix.
+        # 
+        # The prefix must be 2 to 37 characters in length.
+        # 
+        # The prefix can contain letters, digits, and special characters but cannot contain consecutive special characters. The prefix must start with a letter or digit and end with a letter or digit. Valid special characters include underscores (`_`), periods (.), and hyphens (`-`).
+        # 
+        # The complete Alibaba Cloud account name of a member in a resource directory is in the @.aliyunid.com format, such as `alice@rd-3G****.aliyunid.com`.
+        # 
+        # Each name must be unique in the resource directory.
         self.account_name_prefix = account_name_prefix  # type: str
+        # The display name of the member.
+        # 
+        # The name must be 2 to 50 characters in length.
+        # 
+        # The name can contain letters, digits, underscores (\_), periods (.), hyphens (-), and spaces.
+        # 
+        # The name must be unique in the resource directory.
         self.display_name = display_name  # type: str
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id  # type: str
+        # The ID of the billing account. If you leave this parameter empty, the member is used as its own billing account.
         self.payer_account_id = payer_account_id  # type: str
+        # The identity type of the member. Valid values:
+        # 
+        # *   resell: The member is an account for a reseller. This is the default value. A relationship is automatically established between the member and the reseller. The management account of the resource directory must be used as the billing account of the member.
+        # *   non_resell: The member is not an account for a reseller. The member is an account that is not associated with a reseller. You can directly use the account to purchase Alibaba Cloud resources. The member is used as its own billing account.
+        # 
+        # > This parameter is available only for resellers at the international site (alibabacloud.com).
         self.resell_account_type = resell_account_type  # type: str
+        # The tag of the member.
         self.tag = tag  # type: list[CreateResourceAccountRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -1570,23 +1800,36 @@
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class CreateResourceAccountResponseBodyAccount(TeaModel):
     def __init__(self, account_id=None, account_name=None, display_name=None, folder_id=None, join_method=None,
                  join_time=None, modify_time=None, resource_directory_id=None, status=None, type=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
+        # The Alibaba Cloud account name of the member.
         self.account_name = account_name  # type: str
+        # The display name of the member.
         self.display_name = display_name  # type: str
+        # The ID of the folder.
         self.folder_id = folder_id  # type: str
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method  # type: str
+        # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time  # type: str
+        # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time  # type: str
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id  # type: str
+        # The status of the member. The value CreateSuccess indicates that the member is created.
         self.status = status  # type: str
+        # The type of the member. The value ResourceAccount indicates that the member is a resource account.
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateResourceAccountResponseBodyAccount, self).to_map()
@@ -1639,15 +1882,17 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class CreateResourceAccountResponseBody(TeaModel):
     def __init__(self, account=None, request_id=None):
+        # The information of the member.
         self.account = account  # type: CreateResourceAccountResponseBodyAccount
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -1709,14 +1954,15 @@
             temp_model = CreateResourceAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeclineHandshakeRequest(TeaModel):
     def __init__(self, handshake_id=None):
+        # The ID of the invitation.
         self.handshake_id = handshake_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeclineHandshakeRequest, self).to_map()
@@ -1735,24 +1981,44 @@
         return self
 
 
 class DeclineHandshakeResponseBodyHandshake(TeaModel):
     def __init__(self, create_time=None, expire_time=None, handshake_id=None, master_account_id=None,
                  master_account_name=None, modify_time=None, note=None, resource_directory_id=None, status=None, target_entity=None,
                  target_type=None):
+        # The time when the invitation was created.
         self.create_time = create_time  # type: str
+        # The time when the invitation expires.
         self.expire_time = expire_time  # type: str
+        # The ID of the invitation.
         self.handshake_id = handshake_id  # type: str
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id  # type: str
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name  # type: str
+        # The time when the invitation was modified.
         self.modify_time = modify_time  # type: str
+        # The description of the invitation.
         self.note = note  # type: str
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id  # type: str
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status  # type: str
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity  # type: str
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeclineHandshakeResponseBodyHandshake, self).to_map()
@@ -1809,15 +2075,17 @@
         if m.get('TargetType') is not None:
             self.target_type = m.get('TargetType')
         return self
 
 
 class DeclineHandshakeResponseBody(TeaModel):
     def __init__(self, handshake=None, request_id=None):
+        # The information of the invitation.
         self.handshake = handshake  # type: DeclineHandshakeResponseBodyHandshake
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -1879,15 +2147,19 @@
             temp_model = DeclineHandshakeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteAccountRequest(TeaModel):
     def __init__(self, abandonable_check_id=None, account_id=None):
+        # The IDs of the check items that you can choose to ignore for the member deletion.
+        # 
+        # You can obtain the IDs from the response of the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation.
         self.abandonable_check_id = abandonable_check_id  # type: list[str]
+        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteAccountRequest, self).to_map()
@@ -1908,15 +2180,19 @@
         if m.get('AccountId') is not None:
             self.account_id = m.get('AccountId')
         return self
 
 
 class DeleteAccountShrinkRequest(TeaModel):
     def __init__(self, abandonable_check_id_shrink=None, account_id=None):
+        # The IDs of the check items that you can choose to ignore for the member deletion.
+        # 
+        # You can obtain the IDs from the response of the [GetAccountDeletionCheckResult](~~GetAccountDeletionCheckResult~~) operation.
         self.abandonable_check_id_shrink = abandonable_check_id_shrink  # type: str
+        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteAccountShrinkRequest, self).to_map()
@@ -1937,15 +2213,20 @@
         if m.get('AccountId') is not None:
             self.account_id = m.get('AccountId')
         return self
 
 
 class DeleteAccountResponseBody(TeaModel):
     def __init__(self, deletion_type=None, request_id=None):
+        # The type of the deletion. Valid values:
+        # 
+        # *   0: direct deletion. If the member does not have pay-as-you-go resources that are purchased within the previous 30 days, the system directly deletes the member.
+        # *   1: deletion with a silence period. If the member has pay-as-you-go resources that are purchased within the previous 30 days, the member enters a silence period of 45 days. The system starts to delete the member until the silence period ends. For more information about the silence period, see [What is the silence period for member deletion?](~~446079~~)
         self.deletion_type = deletion_type  # type: str
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteAccountResponseBody, self).to_map()
@@ -2005,14 +2286,15 @@
             temp_model = DeleteAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteControlPolicyRequest(TeaModel):
     def __init__(self, policy_id=None):
+        # The ID of the access control policy.
         self.policy_id = policy_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteControlPolicyRequest, self).to_map()
@@ -2029,14 +2311,15 @@
         if m.get('PolicyId') is not None:
             self.policy_id = m.get('PolicyId')
         return self
 
 
 class DeleteControlPolicyResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteControlPolicyResponseBody, self).to_map()
@@ -2092,14 +2375,15 @@
             temp_model = DeleteControlPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteFolderRequest(TeaModel):
     def __init__(self, folder_id=None):
+        # The ID of the folder.
         self.folder_id = folder_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteFolderRequest, self).to_map()
@@ -2116,14 +2400,15 @@
         if m.get('FolderId') is not None:
             self.folder_id = m.get('FolderId')
         return self
 
 
 class DeleteFolderResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteFolderResponseBody, self).to_map()
@@ -2179,15 +2464,20 @@
             temp_model = DeleteFolderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteMessageContactRequest(TeaModel):
     def __init__(self, contact_id=None, retain_contact_in_members=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # Specifies whether to retain the contact for members. Valid values:
+        # 
+        # *   true (default): retains the contact for members. In this case, the contact can still receive messages for the members.
+        # *   false: does not retain the contact for members. In this case, the contact can no longer receive messages for the members. If you set this parameter to false, the response is asynchronously returned. You can call [GetMessageContactDeletionStatus](~~GetMessageContactDeletionStatus~~) to obtain the deletion result.
         self.retain_contact_in_members = retain_contact_in_members  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteMessageContactRequest, self).to_map()
@@ -2208,15 +2498,20 @@
         if m.get('RetainContactInMembers') is not None:
             self.retain_contact_in_members = m.get('RetainContactInMembers')
         return self
 
 
 class DeleteMessageContactResponseBody(TeaModel):
     def __init__(self, request_id=None, status=None):
+        # The request ID.
         self.request_id = request_id  # type: str
+        # The deletion status of the contact. Valid values:
+        # 
+        # *   Deleting
+        # *   Deleted
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeleteMessageContactResponseBody, self).to_map()
@@ -2276,15 +2571,17 @@
             temp_model = DeleteMessageContactResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeregisterDelegatedAdministratorRequest(TeaModel):
     def __init__(self, account_id=None, service_principal=None):
+        # The Alibaba Cloud account ID of the member in the resource directory.
         self.account_id = account_id  # type: str
+        # The identifier of the trusted service.
         self.service_principal = service_principal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeregisterDelegatedAdministratorRequest, self).to_map()
@@ -2305,14 +2602,15 @@
         if m.get('ServicePrincipal') is not None:
             self.service_principal = m.get('ServicePrincipal')
         return self
 
 
 class DeregisterDelegatedAdministratorResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DeregisterDelegatedAdministratorResponseBody, self).to_map()
@@ -2431,15 +2729,21 @@
             temp_model = DestroyResourceDirectoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DetachControlPolicyRequest(TeaModel):
     def __init__(self, policy_id=None, target_id=None):
+        # The ID of the access control policy.
         self.policy_id = policy_id  # type: str
+        # The ID of the object from which you want to detach the access control policy. Access control policies can be attached to the following objects:
+        # 
+        # *   Root folder
+        # *   Subfolders of the Root folder
+        # *   Members
         self.target_id = target_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DetachControlPolicyRequest, self).to_map()
@@ -2460,14 +2764,15 @@
         if m.get('TargetId') is not None:
             self.target_id = m.get('TargetId')
         return self
 
 
 class DetachControlPolicyResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DetachControlPolicyResponseBody, self).to_map()
@@ -2591,15 +2896,17 @@
             temp_model = DisableControlPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DisassociateMembersRequest(TeaModel):
     def __init__(self, contact_id=None, members=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The IDs of objects from which you want to unbind the contact.
         self.members = members  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DisassociateMembersRequest, self).to_map()
@@ -2620,16 +2927,23 @@
         if m.get('Members') is not None:
             self.members = m.get('Members')
         return self
 
 
 class DisassociateMembersResponseBodyMembers(TeaModel):
     def __init__(self, contact_id=None, member_id=None, modify_date=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The ID of the object. Valid values:
+        # 
+        # - ID of the resource directory
+        # - ID of the folder
+        # - ID of the member
         self.member_id = member_id  # type: str
+        # The time when the contact was unbound from the object.
         self.modify_date = modify_date  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DisassociateMembersResponseBodyMembers, self).to_map()
@@ -2654,15 +2968,17 @@
         if m.get('ModifyDate') is not None:
             self.modify_date = m.get('ModifyDate')
         return self
 
 
 class DisassociateMembersResponseBody(TeaModel):
     def __init__(self, members=None, request_id=None):
+        # The time when the contact was unbound from the object.
         self.members = members  # type: list[DisassociateMembersResponseBodyMembers]
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.members:
             for k in self.members:
                 if k:
                     k.validate()
@@ -2798,17 +3114,34 @@
             temp_model = EnableControlPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class EnableResourceDirectoryRequest(TeaModel):
     def __init__(self, enable_mode=None, maname=None, masecure_mobile_phone=None, verification_code=None):
+        # The mode in which you enable a resource directory. Valid values:
+        # 
+        # *   CurrentAccount: The current account is used to enable a resource directory.
+        # *   NewManagementAccount: A newly created account is used to enable a resource directory. If you select this mode, you must configure the `MAName`, `MASecureMobilePhone`, and `VerificationCode` parameters.
         self.enable_mode = enable_mode  # type: str
+        # The name of the newly created account.
+        # 
+        # Specify the name in the `<Prefix>@rdadmin.aliyunid.com` format. The prefix can contain letters, digits, and special characters but cannot contain consecutive special characters. The prefix must start and end with a letter or digit. Valid special characters include underscores (`_`), periods (.), and hyphens (-). The prefix must be 2 to 50 characters in length.
         self.maname = maname  # type: str
+        # The mobile phone number that is bound to the newly created account.
+        # 
+        # If you leave this parameter empty, the mobile phone number that is bound to the current account is used. The mobile phone number you specify must be the same as the mobile phone number that you specify when you call the [SendVerificationCodeForEnableRD](~~SendVerificationCodeForEnableRD~~) operation to obtain a verification code.
+        # 
+        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
+        # 
+        # > Mobile phone numbers in the `86-<Mobile phone number>` format in the Chinese mainland are not supported.
         self.masecure_mobile_phone = masecure_mobile_phone  # type: str
+        # The verification code.
+        # 
+        # You can call the [SendVerificationCodeForEnableRD](~~SendVerificationCodeForEnableRD~~) operation to obtain the verification code.
         self.verification_code = verification_code  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(EnableResourceDirectoryRequest, self).to_map()
@@ -2838,18 +3171,23 @@
             self.verification_code = m.get('VerificationCode')
         return self
 
 
 class EnableResourceDirectoryResponseBodyResourceDirectory(TeaModel):
     def __init__(self, create_time=None, master_account_id=None, master_account_name=None,
                  resource_directory_id=None, root_folder_id=None):
+        # The time when the resource directory was enabled.
         self.create_time = create_time  # type: str
+        # The ID of the management account.
         self.master_account_id = master_account_id  # type: str
+        # The name of the management account.
         self.master_account_name = master_account_name  # type: str
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id  # type: str
+        # The ID of the Root folder.
         self.root_folder_id = root_folder_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(EnableResourceDirectoryResponseBodyResourceDirectory, self).to_map()
@@ -2882,15 +3220,17 @@
         if m.get('RootFolderId') is not None:
             self.root_folder_id = m.get('RootFolderId')
         return self
 
 
 class EnableResourceDirectoryResponseBody(TeaModel):
     def __init__(self, request_id=None, resource_directory=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
+        # The information about the resource directory.
         self.resource_directory = resource_directory  # type: EnableResourceDirectoryResponseBodyResourceDirectory
 
     def validate(self):
         if self.resource_directory:
             self.resource_directory.validate()
 
     def to_map(self):
@@ -2952,15 +3292,20 @@
             temp_model = EnableResourceDirectoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetAccountRequest(TeaModel):
     def __init__(self, account_id=None, include_tags=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
+        # Specifies whether to return the information of tags. Valid values:
+        # 
+        # *   false (default value)
+        # *   true
         self.include_tags = include_tags  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAccountRequest, self).to_map()
@@ -2981,15 +3326,17 @@
         if m.get('IncludeTags') is not None:
             self.include_tags = m.get('IncludeTags')
         return self
 
 
 class GetAccountResponseBodyAccountTags(TeaModel):
     def __init__(self, key=None, value=None):
+        # A tag key.
         self.key = key  # type: str
+        # A tag value.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAccountResponseBodyAccountTags, self).to_map()
@@ -3012,28 +3359,62 @@
         return self
 
 
 class GetAccountResponseBodyAccount(TeaModel):
     def __init__(self, account_id=None, account_name=None, display_name=None, email_status=None, folder_id=None,
                  identity_information=None, join_method=None, join_time=None, location=None, modify_time=None,
                  resource_directory_id=None, resource_directory_path=None, status=None, tags=None, type=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
+        # The Alibaba Cloud account name of the member.
         self.account_name = account_name  # type: str
+        # The display name of the member.
         self.display_name = display_name  # type: str
+        # The status of the modification for the email address bound to the member. Valid values:
+        # 
+        # *   If the value of this parameter is empty, no modification is performed for the email address.
+        # *   WAIT_MODIFY: The modification is being performed.
+        # *   CANCELLED: The modification is canceled.
+        # *   EXPIRED: The modification expires.
         self.email_status = email_status  # type: str
+        # The ID of the folder.
         self.folder_id = folder_id  # type: str
+        # The real-name verification information.
         self.identity_information = identity_information  # type: str
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method  # type: str
+        # The time when the member joined the resource directory.
         self.join_time = join_time  # type: str
+        # The location of the member in the resource directory.
         self.location = location  # type: str
+        # The time when the member was modified.
         self.modify_time = modify_time  # type: str
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id  # type: str
+        # The path of the member in the resource directory.
         self.resource_directory_path = resource_directory_path  # type: str
+        # The status of the member. Valid values:
+        # 
+        # *   CreateSuccess: The member is created.
+        # *   PromoteVerifying: The upgrade of the member is being confirmed.
+        # *   PromoteFailed: The upgrade of the member fails.
+        # *   PromoteExpired: The upgrade of the member expires.
+        # *   PromoteCancelled: The upgrade of the member is canceled.
+        # *   PromoteSuccess: The member is upgraded.
+        # *   InviteSuccess: The member accepts the invitation.
         self.status = status  # type: str
+        # The tags of the member.
         self.tags = tags  # type: list[GetAccountResponseBodyAccountTags]
+        # The type of the member. Valid values:
+        # 
+        # *   CloudAccount: cloud account
+        # *   ResourceAccount: resource account
         self.type = type  # type: str
 
     def validate(self):
         if self.tags:
             for k in self.tags:
                 if k:
                     k.validate()
@@ -3114,15 +3495,17 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class GetAccountResponseBody(TeaModel):
     def __init__(self, account=None, request_id=None):
+        # The information of the member.
         self.account = account  # type: GetAccountResponseBodyAccount
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -3184,14 +3567,15 @@
             temp_model = GetAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetAccountDeletionCheckResultRequest(TeaModel):
     def __init__(self, account_id=None):
+        # The Alibaba Cloud account ID of the member that you want to delete.
         self.account_id = account_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAccountDeletionCheckResultRequest, self).to_map()
@@ -3208,16 +3592,19 @@
         if m.get('AccountId') is not None:
             self.account_id = m.get('AccountId')
         return self
 
 
 class GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoAbandonableChecks(TeaModel):
     def __init__(self, check_id=None, check_name=None, description=None):
+        # The ID of the check item.
         self.check_id = check_id  # type: str
+        # The name of the cloud service to which the check item belongs.
         self.check_name = check_name  # type: str
+        # The description of the check item.
         self.description = description  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoAbandonableChecks, self).to_map()
@@ -3242,16 +3629,19 @@
         if m.get('Description') is not None:
             self.description = m.get('Description')
         return self
 
 
 class GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoNotAllowReason(TeaModel):
     def __init__(self, check_id=None, check_name=None, description=None):
+        # The ID of the check item.
         self.check_id = check_id  # type: str
+        # The name of the cloud service to which the check item belongs.
         self.check_name = check_name  # type: str
+        # The description of the check item.
         self.description = description  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoNotAllowReason, self).to_map()
@@ -3276,17 +3666,31 @@
         if m.get('Description') is not None:
             self.description = m.get('Description')
         return self
 
 
 class GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfo(TeaModel):
     def __init__(self, abandonable_checks=None, allow_delete=None, not_allow_reason=None, status=None):
+        # The check items that you can choose to ignore for the member deletion.
+        # 
+        # > This parameter may be returned if the value of AllowDelete is true.
         self.abandonable_checks = abandonable_checks  # type: list[GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoAbandonableChecks]
+        # Indicates whether the member can be deleted. Valid values:
+        # 
+        # *   true: The member can be deleted.
+        # *   false: The member cannot be deleted.
         self.allow_delete = allow_delete  # type: str
+        # The reasons why the member cannot be deleted.
+        # 
+        # > This parameter is returned only if the value of AllowDelete is false.
         self.not_allow_reason = not_allow_reason  # type: list[GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfoNotAllowReason]
+        # The status of the check. Valid values:
+        # 
+        # *   PreCheckComplete: The check is complete.
+        # *   PreChecking: The check is in progress.
         self.status = status  # type: str
 
     def validate(self):
         if self.abandonable_checks:
             for k in self.abandonable_checks:
                 if k:
                     k.validate()
@@ -3332,15 +3736,17 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class GetAccountDeletionCheckResultResponseBody(TeaModel):
     def __init__(self, account_deletion_check_result_info=None, request_id=None):
+        # The result of the deletion check for the member.
         self.account_deletion_check_result_info = account_deletion_check_result_info  # type: GetAccountDeletionCheckResultResponseBodyAccountDeletionCheckResultInfo
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.account_deletion_check_result_info:
             self.account_deletion_check_result_info.validate()
 
     def to_map(self):
@@ -3402,14 +3808,15 @@
             temp_model = GetAccountDeletionCheckResultResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetAccountDeletionStatusRequest(TeaModel):
     def __init__(self, account_id=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAccountDeletionStatusRequest, self).to_map()
@@ -3426,15 +3833,17 @@
         if m.get('AccountId') is not None:
             self.account_id = m.get('AccountId')
         return self
 
 
 class GetAccountDeletionStatusResponseBodyRdAccountDeletionStatusFailReasonList(TeaModel):
     def __init__(self, description=None, name=None):
+        # The description of the check item.
         self.description = description  # type: str
+        # The name of the cloud service to which the check item belongs.
         self.name = name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAccountDeletionStatusResponseBodyRdAccountDeletionStatusFailReasonList, self).to_map()
@@ -3456,19 +3865,34 @@
             self.name = m.get('Name')
         return self
 
 
 class GetAccountDeletionStatusResponseBodyRdAccountDeletionStatus(TeaModel):
     def __init__(self, account_id=None, create_time=None, deletion_time=None, deletion_type=None,
                  fail_reason_list=None, status=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
+        # The start time of the deletion.
         self.create_time = create_time  # type: str
+        # The end time of the deletion.
         self.deletion_time = deletion_time  # type: str
+        # The type of the deletion. Valid values:
+        # 
+        # *   0: direct deletion. If the member does not have pay-as-you-go resources that are purchased within the previous 30 days, the system directly deletes the member.
+        # *   1: deletion with a silence period. If the member has pay-as-you-go resources that are purchased within the previous 30 days, the member enters a silence period of 45 days. The system starts to delete the member until the silence period ends. For more information about the silence period, see [What is the silence period for member deletion?](~~446079~~)
         self.deletion_type = deletion_type  # type: str
+        # The reasons why the member fails to be deleted.
         self.fail_reason_list = fail_reason_list  # type: list[GetAccountDeletionStatusResponseBodyRdAccountDeletionStatusFailReasonList]
+        # The status. Valid values:
+        # 
+        # *   Success: The member is deleted.
+        # *   Checking: A deletion check is being performed for the member.
+        # *   Deleting: The member is being deleted.
+        # *   CheckFailed: The deletion check for the member fails.
+        # *   DeleteFailed: The member fails to be deleted.
         self.status = status  # type: str
 
     def validate(self):
         if self.fail_reason_list:
             for k in self.fail_reason_list:
                 if k:
                     k.validate()
@@ -3513,15 +3937,17 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class GetAccountDeletionStatusResponseBody(TeaModel):
     def __init__(self, rd_account_deletion_status=None, request_id=None):
+        # The deletion status of the member.
         self.rd_account_deletion_status = rd_account_deletion_status  # type: GetAccountDeletionStatusResponseBodyRdAccountDeletionStatus
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.rd_account_deletion_status:
             self.rd_account_deletion_status.validate()
 
     def to_map(self):
@@ -3583,15 +4009,23 @@
             temp_model = GetAccountDeletionStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetControlPolicyRequest(TeaModel):
     def __init__(self, language=None, policy_id=None):
+        # The language in which you want to return the description of the access control policy. Valid values:
+        # 
+        # *   zh-CN (default value): Chinese
+        # *   en: English
+        # *   ja: Japanese
+        # 
+        # > This parameter is valid only for system access control policies.
         self.language = language  # type: str
+        # The ID of the access control policy.
         self.policy_id = policy_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetControlPolicyRequest, self).to_map()
@@ -3613,22 +4047,37 @@
             self.policy_id = m.get('PolicyId')
         return self
 
 
 class GetControlPolicyResponseBodyControlPolicy(TeaModel):
     def __init__(self, attachment_count=None, create_date=None, description=None, effect_scope=None,
                  policy_document=None, policy_id=None, policy_name=None, policy_type=None, update_date=None):
+        # The number of times that the access control policy is referenced.
         self.attachment_count = attachment_count  # type: str
+        # The time when the access control policy was created.
         self.create_date = create_date  # type: str
+        # The description of the access control policy.
         self.description = description  # type: str
+        # The effective scope of the access control policy. Valid values:
+        # 
+        # *   All: The access control policy is in effect for Alibaba Cloud accounts, RAM users, and RAM roles.
+        # *   RAM: The access control policy is in effect only for RAM users and RAM roles.
         self.effect_scope = effect_scope  # type: str
+        # The document of the access control policy.
         self.policy_document = policy_document  # type: str
+        # The ID of the access control policy.
         self.policy_id = policy_id  # type: str
+        # The name of the access control policy.
         self.policy_name = policy_name  # type: str
+        # The type of the access control policy. Valid values:
+        # 
+        # *   System: system access control policy
+        # *   Custom: custom access control policy
         self.policy_type = policy_type  # type: str
+        # The time when the access control policy was updated.
         self.update_date = update_date  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetControlPolicyResponseBodyControlPolicy, self).to_map()
@@ -3677,15 +4126,17 @@
         if m.get('UpdateDate') is not None:
             self.update_date = m.get('UpdateDate')
         return self
 
 
 class GetControlPolicyResponseBody(TeaModel):
     def __init__(self, control_policy=None, request_id=None):
+        # The details of the access control policy.
         self.control_policy = control_policy  # type: GetControlPolicyResponseBodyControlPolicy
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.control_policy:
             self.control_policy.validate()
 
     def to_map(self):
@@ -3815,14 +4266,15 @@
             temp_model = GetControlPolicyEnablementStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetFolderRequest(TeaModel):
     def __init__(self, folder_id=None):
+        # The ID of the folder.
         self.folder_id = folder_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetFolderRequest, self).to_map()
@@ -3840,18 +4292,23 @@
             self.folder_id = m.get('FolderId')
         return self
 
 
 class GetFolderResponseBodyFolder(TeaModel):
     def __init__(self, create_time=None, folder_id=None, folder_name=None, parent_folder_id=None,
                  resource_directory_path=None):
+        # The time when the folder was created.
         self.create_time = create_time  # type: str
+        # The ID of the folder.
         self.folder_id = folder_id  # type: str
+        # The name of the folder.
         self.folder_name = folder_name  # type: str
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id  # type: str
+        # The path of the folder in the resource directory.
         self.resource_directory_path = resource_directory_path  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetFolderResponseBodyFolder, self).to_map()
@@ -3884,15 +4341,17 @@
         if m.get('ResourceDirectoryPath') is not None:
             self.resource_directory_path = m.get('ResourceDirectoryPath')
         return self
 
 
 class GetFolderResponseBody(TeaModel):
     def __init__(self, folder=None, request_id=None):
+        # The information about the folder.
         self.folder = folder  # type: GetFolderResponseBodyFolder
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.folder:
             self.folder.validate()
 
     def to_map(self):
@@ -3954,14 +4413,15 @@
             temp_model = GetFolderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetHandshakeRequest(TeaModel):
     def __init__(self, handshake_id=None):
+        # The ID of the invitation.
         self.handshake_id = handshake_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetHandshakeRequest, self).to_map()
@@ -3980,26 +4440,52 @@
         return self
 
 
 class GetHandshakeResponseBodyHandshake(TeaModel):
     def __init__(self, create_time=None, expire_time=None, handshake_id=None, invited_account_real_name=None,
                  master_account_id=None, master_account_name=None, master_account_real_name=None, modify_time=None, note=None,
                  resource_directory_id=None, status=None, target_entity=None, target_type=None):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time  # type: str
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time  # type: str
+        # The ID of the invitation.
         self.handshake_id = handshake_id  # type: str
+        # The real-name verification information of the invitee.
+        # 
+        # > This parameter is available only when an invitee calls this operation.
         self.invited_account_real_name = invited_account_real_name  # type: str
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id  # type: str
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name  # type: str
+        # The real-name verification information of the management account of the resource directory.
+        # 
+        # > This parameter is available only when an invitee calls this operation.
         self.master_account_real_name = master_account_real_name  # type: str
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time  # type: str
+        # The description of the invitation.
         self.note = note  # type: str
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id  # type: str
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending: The invitation is waiting for confirmation.
+        # *   Accepted: The invitation is accepted.
+        # *   Cancelled: The invitation is canceled.
+        # *   Declined: The invitation is rejected.
+        # *   Expired: The invitation expires.
         self.status = status  # type: str
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity  # type: str
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetHandshakeResponseBodyHandshake, self).to_map()
@@ -4064,15 +4550,17 @@
         if m.get('TargetType') is not None:
             self.target_type = m.get('TargetType')
         return self
 
 
 class GetHandshakeResponseBody(TeaModel):
     def __init__(self, handshake=None, request_id=None):
+        # The information of the invitation.
         self.handshake = handshake  # type: GetHandshakeResponseBodyHandshake
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -4134,14 +4622,15 @@
             temp_model = GetHandshakeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetMessageContactRequest(TeaModel):
     def __init__(self, contact_id=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetMessageContactRequest, self).to_map()
@@ -4159,22 +4648,35 @@
             self.contact_id = m.get('ContactId')
         return self
 
 
 class GetMessageContactResponseBodyContact(TeaModel):
     def __init__(self, contact_id=None, create_date=None, email_address=None, members=None, message_types=None,
                  name=None, phone_number=None, status=None, title=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The time when the contact was created.
         self.create_date = create_date  # type: str
+        # The email address of the contact.
         self.email_address = email_address  # type: str
+        # The IDs of objects to which the contact is bound.
         self.members = members  # type: list[str]
+        # The types of messages received by the contact.
         self.message_types = message_types  # type: list[str]
+        # The name of the contact.
         self.name = name  # type: str
+        # The mobile phone number of the contact.
         self.phone_number = phone_number  # type: str
+        # The status of the contact. Valid values:
+        # 
+        # *   Verifying
+        # *   Active
+        # *   Deleting
         self.status = status  # type: str
+        # The job title of the contact.
         self.title = title  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetMessageContactResponseBodyContact, self).to_map()
@@ -4223,15 +4725,17 @@
         if m.get('Title') is not None:
             self.title = m.get('Title')
         return self
 
 
 class GetMessageContactResponseBody(TeaModel):
     def __init__(self, contact=None, request_id=None):
+        # The information about the contact.
         self.contact = contact  # type: GetMessageContactResponseBodyContact
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.contact:
             self.contact.validate()
 
     def to_map(self):
@@ -4293,14 +4797,15 @@
             temp_model = GetMessageContactResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetMessageContactDeletionStatusRequest(TeaModel):
     def __init__(self, contact_id=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetMessageContactDeletionStatusRequest, self).to_map()
@@ -4317,15 +4822,17 @@
         if m.get('ContactId') is not None:
             self.contact_id = m.get('ContactId')
         return self
 
 
 class GetMessageContactDeletionStatusResponseBodyContactDeletionStatusFailReasonList(TeaModel):
     def __init__(self, account_id=None, message_types=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
+        # The types of messages received by the contact.
         self.message_types = message_types  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetMessageContactDeletionStatusResponseBodyContactDeletionStatusFailReasonList, self).to_map()
@@ -4346,16 +4853,22 @@
         if m.get('MessageTypes') is not None:
             self.message_types = m.get('MessageTypes')
         return self
 
 
 class GetMessageContactDeletionStatusResponseBodyContactDeletionStatus(TeaModel):
     def __init__(self, contact_id=None, fail_reason_list=None, status=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The types of messages received by the contact.
         self.fail_reason_list = fail_reason_list  # type: list[GetMessageContactDeletionStatusResponseBodyContactDeletionStatusFailReasonList]
+        # The deletion status of the contact. Valid values:
+        # 
+        # *   Deleting
+        # *   Failed
         self.status = status  # type: str
 
     def validate(self):
         if self.fail_reason_list:
             for k in self.fail_reason_list:
                 if k:
                     k.validate()
@@ -4388,15 +4901,17 @@
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
 class GetMessageContactDeletionStatusResponseBody(TeaModel):
     def __init__(self, contact_deletion_status=None, request_id=None):
+        # The deletion information of the contact.
         self.contact_deletion_status = contact_deletion_status  # type: GetMessageContactDeletionStatusResponseBodyContactDeletionStatus
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.contact_deletion_status:
             self.contact_deletion_status.validate()
 
     def to_map(self):
@@ -4690,15 +5205,17 @@
             temp_model = GetResourceDirectoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class InviteAccountToResourceDirectoryRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
+        # The tag key.
         self.key = key  # type: str
+        # The tag value.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(InviteAccountToResourceDirectoryRequestTag, self).to_map()
@@ -4719,18 +5236,28 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class InviteAccountToResourceDirectoryRequest(TeaModel):
     def __init__(self, note=None, parent_folder_id=None, tag=None, target_entity=None, target_type=None):
+        # The description of the invitation.
+        # 
+        # The description can be up to 1,024 characters in length.
         self.note = note  # type: str
+        # The ID of the parent folder.
         self.parent_folder_id = parent_folder_id  # type: str
+        # The tag value.
         self.tag = tag  # type: list[InviteAccountToResourceDirectoryRequestTag]
+        # The ID or logon email address of the account that you want to invite.
         self.target_entity = target_entity  # type: str
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type  # type: str
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -4773,24 +5300,44 @@
         return self
 
 
 class InviteAccountToResourceDirectoryResponseBodyHandshake(TeaModel):
     def __init__(self, create_time=None, expire_time=None, handshake_id=None, master_account_id=None,
                  master_account_name=None, modify_time=None, note=None, resource_directory_id=None, status=None, target_entity=None,
                  target_type=None):
+        # The time when the invitation was created. The time is displayed in UTC.
         self.create_time = create_time  # type: str
+        # The time when the invitation expires. The time is displayed in UTC.
         self.expire_time = expire_time  # type: str
+        # The ID of the invitation.
         self.handshake_id = handshake_id  # type: str
+        # The ID of the management account of the resource directory.
         self.master_account_id = master_account_id  # type: str
+        # The name of the management account of the resource directory.
         self.master_account_name = master_account_name  # type: str
+        # The time when the invitation was modified. The time is displayed in UTC.
         self.modify_time = modify_time  # type: str
+        # The description of the invitation.
         self.note = note  # type: str
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id  # type: str
+        # The status of the invitation. Valid values:
+        # 
+        # *   Pending
+        # *   Accepted
+        # *   Cancelled
+        # *   Declined
+        # *   Expired
         self.status = status  # type: str
+        # The ID or logon email address of the invited account.
         self.target_entity = target_entity  # type: str
+        # The type of the invited account. Valid values:
+        # 
+        # *   Account: indicates the ID of the account.
+        # *   Email: indicates the logon email address of the account.
         self.target_type = target_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(InviteAccountToResourceDirectoryResponseBodyHandshake, self).to_map()
@@ -4847,15 +5394,17 @@
         if m.get('TargetType') is not None:
             self.target_type = m.get('TargetType')
         return self
 
 
 class InviteAccountToResourceDirectoryResponseBody(TeaModel):
     def __init__(self, handshake=None, request_id=None):
+        # The information about the invitation.
         self.handshake = handshake  # type: InviteAccountToResourceDirectoryResponseBodyHandshake
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.handshake:
             self.handshake.validate()
 
     def to_map(self):
@@ -7427,16 +7976,19 @@
             temp_model = ListHandshakesForResourceDirectoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListMessageContactVerificationsRequest(TeaModel):
     def __init__(self, contact_id=None, page_number=None, page_size=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The page number.
         self.page_number = page_number  # type: int
+        # The number of entries per page.
         self.page_size = page_size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListMessageContactVerificationsRequest, self).to_map()
@@ -7461,15 +8013,20 @@
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         return self
 
 
 class ListMessageContactVerificationsResponseBodyContactVerifications(TeaModel):
     def __init__(self, contact_id=None, target=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The object that is used for verification. Valid values:
+        # 
+        # - Mobile phone number
+        # - Email address
         self.target = target  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListMessageContactVerificationsResponseBodyContactVerifications, self).to_map()
@@ -7491,18 +8048,23 @@
             self.target = m.get('Target')
         return self
 
 
 class ListMessageContactVerificationsResponseBody(TeaModel):
     def __init__(self, contact_verifications=None, page_number=None, page_size=None, request_id=None,
                  total_count=None):
+        # The record for the contact to be verified.
         self.contact_verifications = contact_verifications  # type: list[ListMessageContactVerificationsResponseBodyContactVerifications]
+        # The page number.
         self.page_number = page_number  # type: int
+        # The number of entries per page.
         self.page_size = page_size  # type: int
+        # The request ID.
         self.request_id = request_id  # type: str
+        # The total number of entries returned.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.contact_verifications:
             for k in self.contact_verifications:
                 if k:
                     k.validate()
@@ -7582,17 +8144,25 @@
             temp_model = ListMessageContactVerificationsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListMessageContactsRequest(TeaModel):
     def __init__(self, contact_id=None, member=None, page_number=None, page_size=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The ID of the object to which the contact is bound. Valid values:
+        # 
+        # *   ID of the resource directory
+        # *   ID of the folder
+        # *   ID of the member
         self.member = member  # type: str
+        # The page number.
         self.page_number = page_number  # type: int
+        # The number of entries per page.
         self.page_size = page_size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListMessageContactsRequest, self).to_map()
@@ -7622,23 +8192,37 @@
             self.page_size = m.get('PageSize')
         return self
 
 
 class ListMessageContactsResponseBodyContacts(TeaModel):
     def __init__(self, associated_date=None, contact_id=None, create_date=None, email_address=None, members=None,
                  message_types=None, name=None, phone_number=None, status=None, title=None):
+        # The time when the contact was bound to the objects.
         self.associated_date = associated_date  # type: str
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The time when the contact was added.
         self.create_date = create_date  # type: str
+        # The email address of the contact.
         self.email_address = email_address  # type: str
+        # The IDs of objects to which the contact is bound.
         self.members = members  # type: list[str]
+        # The types of messages received by the contact.
         self.message_types = message_types  # type: list[str]
+        # The name of the contact.
         self.name = name  # type: str
+        # The mobile phone number of the contact.
         self.phone_number = phone_number  # type: str
+        # The status of the contact. Valid values:
+        # 
+        # - Verifying
+        # - Active
+        # - Deleting
         self.status = status  # type: str
+        # The job title of the contact.
         self.title = title  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListMessageContactsResponseBodyContacts, self).to_map()
@@ -7691,18 +8275,23 @@
         if m.get('Title') is not None:
             self.title = m.get('Title')
         return self
 
 
 class ListMessageContactsResponseBody(TeaModel):
     def __init__(self, contacts=None, page_number=None, page_size=None, request_id=None, total_count=None):
+        # The time when the contact was bound to the objects.
         self.contacts = contacts  # type: list[ListMessageContactsResponseBodyContacts]
+        # The page number.
         self.page_number = page_number  # type: int
+        # The number of entries per page.
         self.page_size = page_size  # type: int
+        # The request ID.
         self.request_id = request_id  # type: str
+        # The total number of entries returned.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.contacts:
             for k in self.contacts:
                 if k:
                     k.validate()
@@ -8220,16 +8809,28 @@
             temp_model = ListTargetAttachmentsForControlPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListTrustedServiceStatusRequest(TeaModel):
     def __init__(self, admin_account_id=None, page_number=None, page_size=None):
+        # The ID of the management account or delegated administrator account.
+        # 
+        # *   If you set this parameter to the ID of a management account, the trusted services that are enabled within the management account are queried. The default value of this parameter is the ID of an management account.
+        # *   If you set this parameter to the ID of a delegated administrator account, the trusted services that are enabled within the delegated administrator account are queried.
+        # 
+        # For more information about trusted services and delegated administrator accounts, see [Overview of trusted services](~~208133~~) and [Delegated administrator accounts](~~208117~~).
         self.admin_account_id = admin_account_id  # type: str
+        # The number of the page to return.
+        # 
+        # Pages start from page 1. Default value: 1.
         self.page_number = page_number  # type: int
+        # The number of entries to return on each page.
+        # 
+        # Valid values: 1 to 100. Default value: 10.
         self.page_size = page_size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTrustedServiceStatusRequest, self).to_map()
@@ -8254,15 +8855,17 @@
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
         return self
 
 
 class ListTrustedServiceStatusResponseBodyEnabledServicePrincipalsEnabledServicePrincipal(TeaModel):
     def __init__(self, enable_time=None, service_principal=None):
+        # The time when the trusted service was enabled.
         self.enable_time = enable_time  # type: str
+        # The identifier of the trusted service.
         self.service_principal = service_principal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTrustedServiceStatusResponseBodyEnabledServicePrincipalsEnabledServicePrincipal, self).to_map()
@@ -8316,18 +8919,23 @@
                 self.enabled_service_principal.append(temp_model.from_map(k))
         return self
 
 
 class ListTrustedServiceStatusResponseBody(TeaModel):
     def __init__(self, enabled_service_principals=None, page_number=None, page_size=None, request_id=None,
                  total_count=None):
+        # The information about the trusted services that are enabled.
         self.enabled_service_principals = enabled_service_principals  # type: ListTrustedServiceStatusResponseBodyEnabledServicePrincipals
+        # The page number of the returned page.
         self.page_number = page_number  # type: int
+        # The number of entries returned per page.
         self.page_size = page_size  # type: int
+        # The ID of the request.
         self.request_id = request_id  # type: str
+        # The total number of entries returned.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.enabled_service_principals:
             self.enabled_service_principals.validate()
 
     def to_map(self):
@@ -8496,15 +9104,19 @@
             temp_model = MoveAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RegisterDelegatedAdministratorRequest(TeaModel):
     def __init__(self, account_id=None, service_principal=None):
+        # The Alibaba Cloud account ID of the member in the resource directory.
         self.account_id = account_id  # type: str
+        # The identifier of the trusted service.
+        # 
+        # For more information, see the `Trusted service identifier` column in [Supported trusted services](~~208133~~).
         self.service_principal = service_principal  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RegisterDelegatedAdministratorRequest, self).to_map()
@@ -8525,14 +9137,15 @@
         if m.get('ServicePrincipal') is not None:
             self.service_principal = m.get('ServicePrincipal')
         return self
 
 
 class RegisterDelegatedAdministratorResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RegisterDelegatedAdministratorResponseBody, self).to_map()
@@ -8766,15 +9379,19 @@
             temp_model = RetryChangeAccountEmailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SendEmailVerificationForMessageContactRequest(TeaModel):
     def __init__(self, contact_id=None, email_address=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The email address of the contact.
+        # 
+        # The specified email address must be the one you specify when you call [AddMessageContact](~~AddMessageContact~~).
         self.email_address = email_address  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SendEmailVerificationForMessageContactRequest, self).to_map()
@@ -8795,14 +9412,15 @@
         if m.get('EmailAddress') is not None:
             self.email_address = m.get('EmailAddress')
         return self
 
 
 class SendEmailVerificationForMessageContactResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SendEmailVerificationForMessageContactResponseBody, self).to_map()
@@ -8858,15 +9476,21 @@
             temp_model = SendEmailVerificationForMessageContactResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class SendPhoneVerificationForMessageContactRequest(TeaModel):
     def __init__(self, contact_id=None, phone_number=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The mobile phone number of the contact.
+        # 
+        # The value must be in the `<Country code>-<Mobile phone number>` format.
+        # 
+        # The specified mobile phone number must be the one you specify when you call the [AddMessageContact](~~AddMessageContact~~) operation.
         self.phone_number = phone_number  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SendPhoneVerificationForMessageContactRequest, self).to_map()
@@ -8887,14 +9511,15 @@
         if m.get('PhoneNumber') is not None:
             self.phone_number = m.get('PhoneNumber')
         return self
 
 
 class SendPhoneVerificationForMessageContactResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(SendPhoneVerificationForMessageContactResponseBody, self).to_map()
@@ -9530,16 +10155,26 @@
             temp_model = UntagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateAccountRequest(TeaModel):
     def __init__(self, account_id=None, new_account_type=None, new_display_name=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
+        # The new type of the member. Valid values:
+        # 
+        # *   ResourceAccount: resource account
+        # *   CloudAccount: cloud account
+        # 
+        # > You can specify either `NewDisplayName` or `NewAccountType`.
         self.new_account_type = new_account_type  # type: str
+        # The new display name of the member.
+        # 
+        # > You can specify either `NewDisplayName` or `NewAccountType`.
         self.new_display_name = new_display_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateAccountRequest, self).to_map()
@@ -9565,23 +10200,44 @@
             self.new_display_name = m.get('NewDisplayName')
         return self
 
 
 class UpdateAccountResponseBodyAccount(TeaModel):
     def __init__(self, account_id=None, account_name=None, display_name=None, folder_id=None, join_method=None,
                  join_time=None, modify_time=None, resource_directory_id=None, status=None, type=None):
+        # The Alibaba Cloud account ID of the member.
         self.account_id = account_id  # type: str
+        # The Alibaba Cloud account name of the member.
         self.account_name = account_name  # type: str
+        # The display name of the member.
         self.display_name = display_name  # type: str
+        # The ID of the folder.
         self.folder_id = folder_id  # type: str
+        # The way in which the member joins the resource directory. Valid values:
+        # 
+        # *   invited: The member is invited to join the resource directory.
+        # *   created: The member is directly created in the resource directory.
         self.join_method = join_method  # type: str
+        # The time when the member joined the resource directory. The time is displayed in UTC.
         self.join_time = join_time  # type: str
+        # The time when the member was modified. The time is displayed in UTC.
         self.modify_time = modify_time  # type: str
+        # The ID of the resource directory.
         self.resource_directory_id = resource_directory_id  # type: str
+        # The status of the member. Valid values:
+        # 
+        # *   CreateSuccess: The member is created.
+        # *   InviteSuccess: The member accepts the invitation.
+        # *   Removed: The member is removed.
+        # *   SwitchSuccess: The type of the member is switched.
         self.status = status  # type: str
+        # The type of the member. Valid values:
+        # 
+        # *   CloudAccount: cloud account
+        # *   ResourceAccount: resource account
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateAccountResponseBodyAccount, self).to_map()
@@ -9634,15 +10290,17 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class UpdateAccountResponseBody(TeaModel):
     def __init__(self, account=None, request_id=None):
+        # The information of the member.
         self.account = account  # type: UpdateAccountResponseBodyAccount
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.account:
             self.account.validate()
 
     def to_map(self):
@@ -10052,19 +10710,81 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateMessageContactRequest(TeaModel):
     def __init__(self, contact_id=None, email_address=None, message_types=None, name=None, phone_number=None,
                  title=None):
+        # The ID of the contact.
         self.contact_id = contact_id  # type: str
+        # The email address of the contact.
+        # 
+        # After you specify an email address, you need to call [SendEmailVerificationForMessageContact](~~SendEmailVerificationForMessageContact~~) to send verification information to the email address. After the verification is passed, the email address takes effect.
         self.email_address = email_address  # type: str
+        # The types of messages received by the contact.
         self.message_types = message_types  # type: list[str]
+        # The name of the contact.
         self.name = name  # type: str
+        # The mobile phone number of the contact.
+        # 
+        # Specify the mobile phone number in the `<Country code>-<Mobile phone number>` format.
+        # 
+        # After you specify a mobile phone number, you need to call [SendPhoneVerificationForMessageContact](~~SendPhoneVerificationForMessageContact~~) to send verification information to the mobile phone number. After the verification is passed, the mobile phone number takes effect.
         self.phone_number = phone_number  # type: str
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
         self.title = title  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateMessageContactRequest, self).to_map()
@@ -10101,14 +10821,15 @@
         if m.get('Title') is not None:
             self.title = m.get('Title')
         return self
 
 
 class UpdateMessageContactResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(UpdateMessageContactResponseBody, self).to_map()
```

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/PKG-INFO` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-resourcedirectorymaster20220419-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/SOURCES.txt` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/alibabacloud_resourcedirectorymaster20220419_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_resourcedirectorymaster20220419_py2-1.0.2/setup.py` & `alibabacloud_resourcedirectorymaster20220419_py2-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_resourcedirectorymaster20220419_py2.
 
-Created on 04/05/2023
+Created on 26/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_resourcedirectorymaster20220419"
 NAME = "alibabacloud_resourcedirectorymaster20220419_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ResourceDirectoryMaster (20220419) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

