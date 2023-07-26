# Comparing `tmp/alibabacloud_dbs20210101-1.0.2.tar.gz` & `tmp/alibabacloud_dbs20210101-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dbs20210101-1.0.2.tar", last modified: Tue Jan 31 09:19:55 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dbs20210101-1.0.3.tar", last modified: Wed Jul 26 02:56:27 2023, max compression
```

## Comparing `alibabacloud_dbs20210101-1.0.2.tar` & `alibabacloud_dbs20210101-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      107 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    74347 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101/client.py
--rw-r--r--   0 root         (0) root         (0)   109938 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2023-01-31 09:19:55.000000 alibabacloud_dbs20210101-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:56:27.000000 alibabacloud_dbs20210101-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-26 02:56:26.000000 alibabacloud_dbs20210101-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-26 02:56:26.000000 alibabacloud_dbs20210101-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 02:56:26.000000 alibabacloud_dbs20210101-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-26 02:56:27.000000 alibabacloud_dbs20210101-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-26 02:56:26.000000 alibabacloud_dbs20210101-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-26 02:56:26.000000 alibabacloud_dbs20210101-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:56:27.000000 alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-26 02:56:26.000000 alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    74125 2023-07-26 02:56:26.000000 alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101/client.py
+-rw-r--r--   0 root         (0) root         (0)   111567 2023-07-26 02:56:26.000000 alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 02:56:27.000000 alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-26 02:56:27.000000 alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-26 02:56:27.000000 alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 02:56:27.000000 alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-26 02:56:27.000000 alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-26 02:56:27.000000 alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 02:56:27.000000 alibabacloud_dbs20210101-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2023-07-26 02:56:26.000000 alibabacloud_dbs20210101-1.0.3/setup.py
```

### Comparing `alibabacloud_dbs20210101-1.0.2/LICENSE` & `alibabacloud_dbs20210101-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dbs20210101-1.0.2/PKG-INFO` & `alibabacloud_dbs20210101-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dbs20210101
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Dbs (20210101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dbs20210101-1.0.2/README-CN.md` & `alibabacloud_dbs20210101-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dbs20210101-1.0.2/README.md` & `alibabacloud_dbs20210101-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101/client.py` & `alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
     def create_download_with_options(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        For ApsaraDB RDS for MySQL instances that use standard SSDs or enhanced SSDs (ESSDs) and meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: CreateDownloadRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDownloadResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -205,15 +205,15 @@
 
     async def create_download_with_options_async(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        For ApsaraDB RDS for MySQL instances that use standard SSDs or enhanced SSDs (ESSDs) and meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: CreateDownloadRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDownloadResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -259,42 +259,42 @@
         )
 
     def create_download(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        For ApsaraDB RDS for MySQL instances that use standard SSDs or enhanced SSDs (ESSDs) and meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: CreateDownloadRequest
         @return: CreateDownloadResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_download_with_options(request, runtime)
 
     async def create_download_async(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        For ApsaraDB RDS for MySQL instances that use standard SSDs or enhanced SSDs (ESSDs) and meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: CreateDownloadRequest
         @return: CreateDownloadResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_download_with_options_async(request, runtime)
 
     def create_sandbox_instance_with_options(
         self,
         request: dbs_20210101_models.CreateSandboxInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.CreateSandboxInstanceResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: CreateSandboxInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSandboxInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -339,15 +339,15 @@
 
     async def create_sandbox_instance_with_options_async(
         self,
         request: dbs_20210101_models.CreateSandboxInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.CreateSandboxInstanceResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: CreateSandboxInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSandboxInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -391,42 +391,42 @@
         )
 
     def create_sandbox_instance(
         self,
         request: dbs_20210101_models.CreateSandboxInstanceRequest,
     ) -> dbs_20210101_models.CreateSandboxInstanceResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: CreateSandboxInstanceRequest
         @return: CreateSandboxInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_sandbox_instance_with_options(request, runtime)
 
     async def create_sandbox_instance_async(
         self,
         request: dbs_20210101_models.CreateSandboxInstanceRequest,
     ) -> dbs_20210101_models.CreateSandboxInstanceResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: CreateSandboxInstanceRequest
         @return: CreateSandboxInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_sandbox_instance_with_options_async(request, runtime)
 
     def delete_sandbox_instance_with_options(
         self,
         request: dbs_20210101_models.DeleteSandboxInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DeleteSandboxInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSandboxInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -455,15 +455,15 @@
 
     async def delete_sandbox_instance_with_options_async(
         self,
         request: dbs_20210101_models.DeleteSandboxInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DeleteSandboxInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSandboxInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -491,28 +491,28 @@
         )
 
     def delete_sandbox_instance(
         self,
         request: dbs_20210101_models.DeleteSandboxInstanceRequest,
     ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DeleteSandboxInstanceRequest
         @return: DeleteSandboxInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_sandbox_instance_with_options(request, runtime)
 
     async def delete_sandbox_instance_async(
         self,
         request: dbs_20210101_models.DeleteSandboxInstanceRequest,
     ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DeleteSandboxInstanceRequest
         @return: DeleteSandboxInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_sandbox_instance_with_options_async(request, runtime)
 
@@ -523,16 +523,14 @@
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryBackupSetResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDBTablesRecoveryBackupSet',
             version='2021-01-01',
             protocol='HTTPS',
@@ -555,16 +553,14 @@
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryBackupSetResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDBTablesRecoveryBackupSet',
             version='2021-01-01',
             protocol='HTTPS',
@@ -601,16 +597,14 @@
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryStateResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDBTablesRecoveryState',
             version='2021-01-01',
             protocol='HTTPS',
@@ -633,16 +627,14 @@
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryStateResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDBTablesRecoveryState',
             version='2021-01-01',
             protocol='HTTPS',
@@ -679,16 +671,14 @@
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryTimeRangeResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDBTablesRecoveryTimeRange',
             version='2021-01-01',
             protocol='HTTPS',
@@ -711,16 +701,14 @@
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryTimeRangeResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeDBTablesRecoveryTimeRange',
             version='2021-01-01',
             protocol='HTTPS',
@@ -752,15 +740,15 @@
 
     def describe_download_backup_set_storage_info_with_options(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -795,15 +783,15 @@
 
     async def describe_download_backup_set_storage_info_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -837,42 +825,42 @@
         )
 
     def describe_download_backup_set_storage_info(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_download_backup_set_storage_info_with_options(request, runtime)
 
     async def describe_download_backup_set_storage_info_async(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_download_backup_set_storage_info_with_options_async(request, runtime)
 
     def describe_download_support_with_options(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadSupportRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadSupportResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -901,15 +889,15 @@
 
     async def describe_download_support_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadSupportRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadSupportResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -937,42 +925,42 @@
         )
 
     def describe_download_support(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadSupportRequest
         @return: DescribeDownloadSupportResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_download_support_with_options(request, runtime)
 
     async def describe_download_support_async(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the download destination to an URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadSupportRequest
         @return: DescribeDownloadSupportResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_download_support_with_options_async(request, runtime)
 
     def describe_download_task_with_options(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1021,15 +1009,15 @@
 
     async def describe_download_task_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1077,42 +1065,42 @@
         )
 
     def describe_download_task(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadTaskRequest
         @return: DescribeDownloadTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_download_task_with_options(request, runtime)
 
     async def describe_download_task_async(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        You can create an advanced download task by point in time or backup file. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Advanced download](~~98819~~).
+        You can create an advanced download task by point in time or backup set. You can set the Download Destination parameter to URL or directly upload the downloaded data to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving. For more information, see [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~).
         
         @param request: DescribeDownloadTaskRequest
         @return: DescribeDownloadTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_download_task_with_options_async(request, runtime)
 
     def describe_sandbox_backup_sets_with_options(
         self,
         request: dbs_20210101_models.DescribeSandboxBackupSetsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxBackupSetsResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxBackupSetsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxBackupSetsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1145,15 +1133,15 @@
 
     async def describe_sandbox_backup_sets_with_options_async(
         self,
         request: dbs_20210101_models.DescribeSandboxBackupSetsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxBackupSetsResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxBackupSetsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxBackupSetsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1185,42 +1173,42 @@
         )
 
     def describe_sandbox_backup_sets(
         self,
         request: dbs_20210101_models.DescribeSandboxBackupSetsRequest,
     ) -> dbs_20210101_models.DescribeSandboxBackupSetsResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxBackupSetsRequest
         @return: DescribeSandboxBackupSetsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_sandbox_backup_sets_with_options(request, runtime)
 
     async def describe_sandbox_backup_sets_async(
         self,
         request: dbs_20210101_models.DescribeSandboxBackupSetsRequest,
     ) -> dbs_20210101_models.DescribeSandboxBackupSetsResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxBackupSetsRequest
         @return: DescribeSandboxBackupSetsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_sandbox_backup_sets_with_options_async(request, runtime)
 
     def describe_sandbox_instances_with_options(
         self,
         request: dbs_20210101_models.DescribeSandboxInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxInstancesResponse:
         """
-        The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxInstancesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxInstancesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1253,15 +1241,15 @@
 
     async def describe_sandbox_instances_with_options_async(
         self,
         request: dbs_20210101_models.DescribeSandboxInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxInstancesResponse:
         """
-        The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxInstancesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxInstancesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1293,42 +1281,42 @@
         )
 
     def describe_sandbox_instances(
         self,
         request: dbs_20210101_models.DescribeSandboxInstancesRequest,
     ) -> dbs_20210101_models.DescribeSandboxInstancesResponse:
         """
-        The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxInstancesRequest
         @return: DescribeSandboxInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_sandbox_instances_with_options(request, runtime)
 
     async def describe_sandbox_instances_async(
         self,
         request: dbs_20210101_models.DescribeSandboxInstancesRequest,
     ) -> dbs_20210101_models.DescribeSandboxInstancesResponse:
         """
-        The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxInstancesRequest
         @return: DescribeSandboxInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_sandbox_instances_with_options_async(request, runtime)
 
     def describe_sandbox_recovery_time_with_options(
         self,
         request: dbs_20210101_models.DescribeSandboxRecoveryTimeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxRecoveryTimeResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxRecoveryTimeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxRecoveryTimeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1355,15 +1343,15 @@
 
     async def describe_sandbox_recovery_time_with_options_async(
         self,
         request: dbs_20210101_models.DescribeSandboxRecoveryTimeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxRecoveryTimeResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxRecoveryTimeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxRecoveryTimeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1389,28 +1377,28 @@
         )
 
     def describe_sandbox_recovery_time(
         self,
         request: dbs_20210101_models.DescribeSandboxRecoveryTimeRequest,
     ) -> dbs_20210101_models.DescribeSandboxRecoveryTimeResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxRecoveryTimeRequest
         @return: DescribeSandboxRecoveryTimeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_sandbox_recovery_time_with_options(request, runtime)
 
     async def describe_sandbox_recovery_time_async(
         self,
         request: dbs_20210101_models.DescribeSandboxRecoveryTimeRequest,
     ) -> dbs_20210101_models.DescribeSandboxRecoveryTimeResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Create a sandbox instance for emergency disaster recovery of an ApsaraDB RDS for MySQL database](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). The API operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxRecoveryTimeRequest
         @return: DescribeSandboxRecoveryTimeResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_sandbox_recovery_time_with_options_async(request, runtime)
 
@@ -1423,16 +1411,14 @@
         query = {}
         if not UtilClient.is_unset(request.category):
             query['Category'] = request.category
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.retention):
             query['Retention'] = request.retention
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDBTablesRecoveryState',
@@ -1459,16 +1445,14 @@
         query = {}
         if not UtilClient.is_unset(request.category):
             query['Category'] = request.category
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.retention):
             query['Retention'] = request.retention
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDBTablesRecoveryState',
@@ -1507,16 +1491,14 @@
     ) -> dbs_20210101_models.SupportDBTableRecoveryResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SupportDBTableRecovery',
             version='2021-01-01',
             protocol='HTTPS',
@@ -1539,16 +1521,14 @@
     ) -> dbs_20210101_models.SupportDBTableRecoveryResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='SupportDBTableRecovery',
             version='2021-01-01',
             protocol='HTTPS',
```

### Comparing `alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101/models.py` & `alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,21 @@
     def __init__(
         self,
         client_token: str = None,
         new_resource_group_id: str = None,
         resource_id: str = None,
         resource_type: str = None,
     ):
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token
+        # The ID of the resource group to which you want to move the resource.
         self.new_resource_group_id = new_resource_group_id
+        # The ID of the resource.
         self.resource_id = resource_id
+        # The type of the resource. Set the value to backupplan.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -56,20 +60,33 @@
         data: str = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
+        # The status code returned.
         self.code = code
+        # Indicates whether the resource was successfully moved. Valid values:
+        # 
+        # *   **true**: The resource was successfully moved.
+        # *   **false**: The resource failed to be moved.
         self.data = data
+        # The error code returned if the request failed.
         self.err_code = err_code
+        # The error message returned if the request failed.
         self.err_message = err_message
+        # The additional information.
         self.message = message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request was successful. Valid values:
+        # 
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -167,53 +184,55 @@
         instance_name: str = None,
         region_code: str = None,
         target_bucket: str = None,
         target_oss_region: str = None,
         target_path: str = None,
         target_type: str = None,
     ):
-        # The ID of the backup set. You can call the [DescribeBackups](~~26273~~) operation to obtain the ID of the backup set.
+        # The ID of the backup set. You can call the [DescribeBackups](~~26273~~) operation to query the ID of the backup set.
         # 
-        # >  This parameter is required if the BakSetType parameter is set to full.
+        # > This parameter is required if the BakSetType parameter is set to full.
         self.bak_set_id = bak_set_id
-        # The size of the full backup set. You can call the [DescribeBackups](~~26273~~) operation to query the size of the full backup set. Unit: bytes.
+        # The size of the full backup set. Unit: bytes. You can call the [DescribeBackups](~~26273~~) operation to query the size of the full backup set.
         self.bak_set_size = bak_set_size
         # The type of the download task. Valid values:
         # 
         # *   **full**: downloads a full backup set.
         # *   **pitr**: downloads a backup set at a specific point in time.
         self.bak_set_type = bak_set_type
-        # The point in time at which the backup set is downloaded. The UNIX timestamp of the LONG type. Unit: milliseconds.
+        # The point in time at which the backup set is downloaded. Specify a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         # 
-        # >  This parameter is required if the BakSetType parameter is set to pitr.
+        # > This parameter is required if the BakSetType parameter is set to pitr.
         self.download_point_in_time = download_point_in_time
-        # The destination format to which the downloaded backup set is converted. Valid values:
+        # The format to which the downloaded backup set is converted. Valid values:
         # 
-        # *   **csv**\
+        # *   **CSV**\
         # *   **SQL**\
         # *   **Parquet**\
+        # 
+        # > This parameter is required.
         self.format_type = format_type
         # The ID of the instance.
         self.instance_name = instance_name
         # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](~~26231~~) operation to query the region ID of the instance.
         self.region_code = region_code
         # The name of the OSS bucket that is used to store the backup set.
         # 
         # *   This parameter is required if the TargetType parameter is set to OSS.
-        # *   Make sure that your account has the **AliyunDBSDefaultRole** permission. For more information, see [Use RAM for resource authorization](~~26307~~). You can also grant permissions based on the operation instructions in the RAM console.
+        # *   Make sure that your account is granted the **AliyunDBSDefaultRole** permission. For more information, see [Use RAM for resource authorization](~~26307~~). You can also grant permissions based on the operation instructions in the Resource Access Management (RAM) console.
         self.target_bucket = target_bucket
         # The region in which the OSS bucket resides.
         # 
-        # >  This parameter is required if the TargetType parameter is set to OSS.
+        # > This parameter is required if the TargetType parameter is set to OSS.
         self.target_oss_region = target_oss_region
-        # The destination path of the downloaded data.
+        # The destination path to which the backup set is downloaded.
         # 
-        # >  This parameter is required if the TargetType parameter is set to OSS.
+        # > This parameter is required if the TargetType parameter is set to OSS.
         self.target_path = target_path
-        # The type of the method in which the backup set is downloaded. Valid values:
+        # The type of the destination to which the backup set is downloaded. Valid values:
         # 
         # *   **OSS**\
         # *   **URL**\
         self.target_type = target_type
 
     def validate(self):
         pass
@@ -288,50 +307,50 @@
         import_data_size: int = None,
         progress: str = None,
         region_code: str = None,
         target_path: str = None,
         target_type: str = None,
         task_id: str = None,
     ):
-        # The point in time of the backup set if the task is used to download a backup set at a specific point in time. The value is a timestamp.
+        # The point in time of the backup set if the task is used to download a backup set at a specific point in time. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.backup_set_time = backup_set_time
         # The ID of the full backup set.
         self.bak_set_id = bak_set_id
-        # The database and table information that is returned if the download task is a database and table filtering task.
+        # The database and table information that is returned if databases and tables are filtered by the download task.
         self.db_list = db_list
-        # The status of the download task. Valid values:
+        # The state of the download task. Valid values:
         # 
-        # *   Initializing: The download task is being initialized.
-        # *   queuing: The download task is queuing.
-        # *   running: The download task is running.
-        # *   failed: The download task fails.
-        # *   finished: The download task is complete.
-        # *   expired: The download task expires.
+        # *   initializing: The download task was being initialized.
+        # *   queuing: The download task was queuing.
+        # *   running: The download task was running.
+        # *   failed: The download task failed.
+        # *   finished: The download task was complete.
+        # *   expired: The download task expired.
         # 
-        # >  The download task expires in three days after the task is complete if the TargetType parameter is set to URL.
+        # > If the TargetType parameter is set to URL, the download task expires in three days after the task is complete.
         self.download_status = download_status
-        # The amount of output data. Unit: bytes.
+        # The size of the downloaded data. Unit: bytes.
         self.export_data_size = export_data_size
         # The format to which the downloaded data is converted.
         self.format = format
-        # The time when the download task was created. The value is a timestamp.
+        # The time when the download task was created. This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.gmt_create = gmt_create
-        # The amount of data that is processed. Unit: bytes.
+        # The size of the processed data. Unit: bytes.
         self.import_data_size = import_data_size
         # The number of tables that have been downloaded and the total number of tables to be downloaded.
         # 
-        # >  If the task is in the preparation stage, 0/0 is returned.
+        # > If the task is in the preparation stage, 0/0 is returned.
         self.progress = progress
         # The ID of the region in which the instance resides.
         self.region_code = region_code
-        # The destination path of the downloaded data.
+        # The destination path to which the backup set is downloaded.
         # 
-        # >  This parameter is returned if the TargetType parameter is set to OSS.
+        # > This parameter is returned if the TargetType parameter is set to OSS.
         self.target_path = target_path
-        # The type of the method in which the backup set is downloaded.
+        # The type of the destination to which the backup set is downloaded.
         self.target_type = target_type
         # The ID of the download task.
         self.task_id = task_id
 
     def validate(self):
         pass
 
@@ -407,30 +426,30 @@
         data: CreateDownloadResponseBodyData = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code.
+        # The status code returned.
         self.code = code
-        # The response parameters.
+        # The returned data.
         self.data = data
-        # The error code.
+        # The error code returned if the request failed.
         self.err_code = err_code
-        # The error message.
+        # The error message returned if the request failed.
         self.err_message = err_message
-        # The error message.
+        # The error message returned if the request failed.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful. Valid values:
+        # Indicates whether the request was successful. Valid values:
         # 
-        # *   **true**: The request is successful.
-        # *   **false**: The request fails.
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -531,52 +550,52 @@
         sandbox_type: str = None,
         sandbox_user: str = None,
         vpc_id: str = None,
         vpc_switch_id: str = None,
     ):
         # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to obtain the ID of the backup schedule.
         # 
-        # >  If your instance is an ApsaraDB RDS for MySQL instance, you can configure [automatic access to the instance](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
         self.backup_plan_id = backup_plan_id
         # The ID of the backup set to be restored, which is the point in time when a snapshot was created. You can call the [DescribeSandboxBackupSets](~~437256~~) operation to obtain the ID.
         # 
-        # >  You need to specify only one of the **BackupSetId** and **RestoreTime** parameters.
+        # > You need to specify only one of the **BackupSetId** and **RestoreTime** parameters.
         self.backup_set_id = backup_set_id
         # The point in time of the sandbox instance to be restored. You can call the [DescribeSandboxRecoveryTime](~~437258~~) operation to view the recoverable time range. Specify the time in the format of *yyyy-MM-ddTHH:mm:ssZ*. The time must be in UTC.
         self.restore_time = restore_time
-        # The name of the sandbox instance.
+        # The custom name of the sandbox instance.
         self.sandbox_instance_name = sandbox_instance_name
         # The password of the privileged account created in the sandbox instance.
         self.sandbox_password = sandbox_password
         # The specifications of the sandbox instance. Valid values:
         # 
         # *   **MYSQL\_1C\_1M_SD**: 1 CPU core and 1 GB of memory.
         # *   **MYSQL\_1C\_2M_SD**: 1 CPU core and 2 GB of memory.
         # *   **MYSQL\_2C\_4M_SD**: 2 CPU cores and 4 GB of memory.
         # *   **MYSQL\_2C\_8M_SD**: 2 CPU cores and 8 GB of memory.
         # *   **MYSQL\_4C\_8M_SD**: 4 CPU cores and 8 GB of memory.
         # *   **MYSQL\_4C\_16M_SD**: 4 CPU cores and 16 GB of memory.
         # *   **MYSQL\_8C\_16M_SD**: 8 CPU cores and 16 GB of memory.
         # *   **MYSQL\_8C\_32M_SD**: 8 CPU cores and 32 GB of memory.
         # 
-        # >  Different specifications have little impact on the recovery speed. High-specification instances provide better performance after restoration. For more information, see [Sandbox instance fees](~~201466~~).
+        # > Different specifications have little impact on the recovery speed. High-specification instances provide better performance after restoration. For more information, see [DBS sandbox fees](~~201466~~).
         self.sandbox_specification = sandbox_specification
         # The type of the sandbox instance. You can call this operation only to create an instance of the **Sandbox** type. After the sandbox instance is created, the MySQL endpoint of the instance is provided.
         self.sandbox_type = sandbox_type
         # The privileged account created in the sandbox instance.
         # 
-        # *   After you specify this parameter, the system creates a privileged account in the sandbox instance. The account has the permissions on all databases in the instance.
+        # *   After you specify this parameter, the system creates a privileged account in the sandbox instance. The account is granted the permissions on all databases in the instance.
         # 
         # The account of the source database is retained in the sandbox instance.
         # 
         # *   If you do not specify this parameter, the database account is the same as that of the source database.
         self.sandbox_user = sandbox_user
         # The ID of the virtual private cloud (VPC) that is used to connect to the sandbox instance. If you want to connect to the sandbox instance by using Elastic Compute Service (ECS) instances, you must set this parameter to the VPC in which the ECS instances reside.
         # 
-        # >  You can set this parameter if you want to use it in a recovery drill scenario.
+        # > You can set this parameter if you want to use it in a recovery drill scenario.
         self.vpc_id = vpc_id
         # The ID of the VSwitch that is used to connect to the sandbox instance.
         self.vpc_switch_id = vpc_switch_id
 
     def validate(self):
         pass
 
@@ -635,15 +654,15 @@
 
 class CreateSandboxInstanceResponseBodyData(TeaModel):
     def __init__(
         self,
         backup_plan_id: str = None,
         instance_id: str = None,
     ):
-        # The ID of the backup schedule.
+        # The ID of the backup plan.
         self.backup_plan_id = backup_plan_id
         # The ID of the sandbox instance.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
@@ -675,27 +694,27 @@
         data: CreateSandboxInstanceResponseBodyData = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code.
+        # The error code returned if the request fails.
         self.code = code
         # The response parameters.
         self.data = data
-        # The error code.
+        # The error code returned if the request fails.
         self.err_code = err_code
-        # The error message.
+        # The error message returned if the request fails.
         self.err_message = err_message
-        # The error message.
+        # The error message returned if the request fails.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful.
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -786,19 +805,19 @@
 
 class DeleteSandboxInstanceRequest(TeaModel):
     def __init__(
         self,
         backup_plan_id: str = None,
         instance_id: str = None,
     ):
-        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to obtain the ID of the backup schedule.
+        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to query the ID of the backup schedule.
         # 
-        # >  If your instance is an ApsaraDB RDS for MySQL instance, you can configure [automatic access to the instance](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
         self.backup_plan_id = backup_plan_id
-        # The ID of the sandbox instance. You can call the [DescribeSandboxInstances](~~437257~~) operation to obtain the ID of the sandbox instance.
+        # The ID of the sandbox instance. You can call the [DescribeSandboxInstances](~~437257~~) operation to query the ID of the sandbox instance.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -828,27 +847,27 @@
         data: str = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code.
+        # The error code returned if the request failed.
         self.code = code
-        # The response parameters.
+        # The returned data.
         self.data = data
-        # The error code.
+        # The error code returned if the request failed.
         self.err_code = err_code
-        # The error message.
+        # The error message returned if the request failed.
         self.err_message = err_message
-        # The error message.
+        # The error message returned if the request failed.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful.
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -936,45 +955,39 @@
 
 
 class DescribeDBTablesRecoveryBackupSetRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_code: str = None,
-        region_id: str = None,
     ):
         self.instance_id = instance_id
         self.region_code = region_code
-        self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.region_code is not None:
             result['RegionCode'] = self.region_code
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionCode') is not None:
             self.region_code = m.get('RegionCode')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
         return self
 
 
 class DescribeDBTablesRecoveryBackupSetResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
@@ -1082,45 +1095,39 @@
 
 
 class DescribeDBTablesRecoveryStateRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_code: str = None,
-        region_id: str = None,
     ):
         self.instance_id = instance_id
         self.region_code = region_code
-        self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.region_code is not None:
             result['RegionCode'] = self.region_code
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionCode') is not None:
             self.region_code = m.get('RegionCode')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
         return self
 
 
 class DescribeDBTablesRecoveryStateResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
@@ -1228,45 +1235,39 @@
 
 
 class DescribeDBTablesRecoveryTimeRangeRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_code: str = None,
-        region_id: str = None,
     ):
         self.instance_id = instance_id
         self.region_code = region_code
-        self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.region_code is not None:
             result['RegionCode'] = self.region_code
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionCode') is not None:
             self.region_code = m.get('RegionCode')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
         return self
 
 
 class DescribeDBTablesRecoveryTimeRangeResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
@@ -1380,30 +1381,30 @@
         duration: str = None,
         instance_name: str = None,
         region_code: str = None,
         task_id: str = None,
     ):
         # The ID of the backup set.
         self.backup_set_id = backup_set_id
-        # Set this parameter if the Download Destination parameter is set to URL.
+        # The validity period of the URL that is used as the download destination. Take note of the following items:
         # 
-        # *   By default, a URL is valid for 2 hours, which is equal to 7,200 seconds.
-        # *   The valid duration is 5 minutes (300 seconds) to 1 day (86,400 seconds).
-        # *   Before you set this parameter, convert the time to seconds. For example, if you want to set the validity period of the link to 5 minutes, enter 300.
+        # *   Default value: 7200. This means that the URL is valid for 2 hours by default.
+        # *   Valid values: 300 to 86400. Unit: seconds. This means that you can specify a validity period in the range of 5 minutes to 1 day.
+        # *   Before you specify this parameter, convert the validity period to seconds. For example, if you want to set the validity period of the URL to 5 minutes, enter 300.
         self.duration = duration
         # The ID of the instance.
         # 
-        # >  The **BackupSetId** parameter is required if you specify the **InstanceName** parameter.
+        # > The **BackupSetId** parameter is required if you specify the **InstanceName** parameter.
         self.instance_name = instance_name
-        # The region ID of the instance. You can call the [DescribeDBInstanceAttribute](~~26231~~) operation to query the region ID of the instance.
+        # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](~~26231~~) operation to query the region ID of the instance.
         self.region_code = region_code
         # The ID of the download task.
         # 
         # *   The **BackupSetId** and **InstanceName** parameters are required if you do not specify the **TaskId** parameter.
-        # *   You can find the instance and click **Backup and Restoration**. On the **Backup Download** tab, view the **task ID**.
+        # *   You can go to the instance details page in the Alibaba Cloud Management Console and click **Backup and Restoration** in the left-side navigation pane. On the **Backup Download** tab, view the task ID.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1441,17 +1442,17 @@
 class DescribeDownloadBackupSetStorageInfoResponseBodyData(TeaModel):
     def __init__(
         self,
         expiration_time: int = None,
         private_url: str = None,
         public_url: str = None,
     ):
-        # The expiration time of the URL.
+        # The validity period of the URL.
         # 
-        # >  The return value is in the timestamp format.
+        # > This value is a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
         self.expiration_time = expiration_time
         # The private download URL of the backup set.
         self.private_url = private_url
         # The public download URL of the backup set.
         self.public_url = public_url
 
     def validate(self):
@@ -1489,30 +1490,30 @@
         data: DescribeDownloadBackupSetStorageInfoResponseBodyData = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code.
+        # The error code returned if the request failed.
         self.code = code
-        # The response parameters.
+        # The returned data.
         self.data = data
-        # The error code.
+        # The error code returned if the request failed.
         self.err_code = err_code
-        # The error message.
+        # The error message returned if the request failed.
         self.err_message = err_message
-        # The error message.
+        # The error message returned if the request failed.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request was successful. Valid values:
         # 
-        # *   **true**: the request is successful.
-        # *   **false**: the request fails.
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -1643,33 +1644,33 @@
         data: str = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code.
+        # The error code returned if the request failed.
         self.code = code
         # Indicates whether the advanced download feature is supported. Valid values:
         # 
         # *   **true**: The advanced download feature is supported.
         # *   **false**: The advanced download feature is not supported.
         self.data = data
-        # The error code returned if the request fails.
+        # The error code returned if the request failed.
         self.err_code = err_code
-        # The error message returned if the request fails.
+        # The error message returned if the request failed.
         self.err_message = err_message
-        # The error message.
+        # The error message returned if the request failed.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful. Valid values:
+        # Indicates whether the request was successful. Valid values:
         # 
-        # *   **true**: The request is successful.
-        # *   **false**: The request fails.
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1768,44 +1769,47 @@
         order_direct: str = None,
         page_size: str = None,
         region_code: str = None,
         start_time: str = None,
         state: str = None,
         task_type: str = None,
     ):
-        # The ID of the backup set generated when you create the download task. You can call the [DescribeBackups](~~26273~~) operation to query the backup set ID. Unit: bytes.
+        # The ID of the backup set generated when you create a download task. You can call the [DescribeBackups](~~26273~~) operation to query the ID.
         self.backup_set_id = backup_set_id
         # The page number of the page to return.
         self.current_page = current_page
         # The ID of the Database Backup (DBS) data source. Specify the parameter in the format of *ds-${Instance ID}\_${regionId}*.
         self.datasource_id = datasource_id
         # The end of the time range to query. Specify this parameter as a timestamp of the LONG type. Unit: milliseconds.
         self.end_time = end_time
         # The ID of the instance.
+        # 
+        # > This parameter is required.
         self.instance_name = instance_name
-        # The column based on which the entries are sorted. By default, the entries are sorted by the creation time. Set the value to **gmt_create**.
+        # The column based on which the entries are sorted. By default, the entries are sorted by the time when the download task was created. Set the value to **gmt_create**.
         self.order_column = order_column
         # The order in which you want to sort the entries. Valid values:
         # 
-        # *   **asc**: sorts the retrieved entries by time in ascending order.
-        # *   **desc**: sorts the retrieved entries by time in descending order. This is the default value.
+        # *   **asc**: the ascending order.
+        # *   **desc**: the descending order. This is the default value.
         self.order_direct = order_direct
         # The number of entries to return on each page.
         self.page_size = page_size
         # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](~~26231~~) operation to query the region ID of the instance.
         self.region_code = region_code
         # The beginning of the time range to query. Specify this parameter as a timestamp of the LONG type. Unit: milliseconds.
         self.start_time = start_time
-        # The status of the download task. Valid values:
+        # The state of the download task. Valid values:
         # 
         # *   **Initializing**: The download task is being initialized.
         # *   **queuing**: The download task is queuing.
         # *   **running**: The download task is running.
         # *   **failed**: The download task fails.
         # *   **finished**: The download task is complete.
+        # *   **expired**: The download task expires.
         self.state = state
         # The type of the download task. Valid values:
         # 
         # *   **full**: downloads a full backup set.
         # *   **pitr**: downloads a backup set at a specific point in time.
         self.task_type = task_type
 
@@ -1890,24 +1894,24 @@
         target_type: str = None,
         task_id: str = None,
     ):
         # The point in time of the backup set if the task is used to download a backup set at a specific point in time. The value is a timestamp of the LONG type. Unit: milliseconds.
         self.backup_set_time = backup_set_time
         # The ID of the full backup set.
         self.bak_set_id = bak_set_id
-        # The details of the databases.
+        # The databases.
         self.db_list = db_list
-        # The status of the download task. Valid values:
+        # The state of the download task. Valid values:
         # 
-        # *   **Initializing**: The download task is being initialized.
-        # *   **queuing**: The download task is queuing.
-        # *   **running**: The download task is running.
-        # *   **failed**: The download task fails.
-        # *   **finished**: The download task is complete.
-        # *   **expired**: The download task expires.
+        # *   **Initializing**: The download task was being initialized.
+        # *   **queuing**: The download task was queuing.
+        # *   **running**: The download task was running.
+        # *   **failed**: The download task failed.
+        # *   **finished**: The download task was complete.
+        # *   **expired**: The download task expired.
         self.download_status = download_status
         # The amount of output data. Unit: bytes.
         self.export_data_size = export_data_size
         # The format to which the downloaded backup set is converted. Valid values:
         # 
         # *   **csv**\
         # *   **SQL**\
@@ -2040,20 +2044,23 @@
         content: DescribeDownloadTaskResponseBodyDataContent = None,
         extra: str = None,
         page_number: int = None,
         page_size: int = None,
         total_elements: int = None,
         total_pages: int = None,
     ):
-        # The details of the download tasks.
+        # The details of the download task.
         self.content = content
-        # The extra description of the download task.
+        # The extra description of the download tasks.
         self.extra = extra
+        # The page number of the returned page. The value must be an integer that is greater than 0. Default value: 1.
         self.page_number = page_number
+        # The number of entries returned per page.
         self.page_size = page_size
+        # The total number of full backup tasks.
         self.total_elements = total_elements
         # The total number of returned pages.
         self.total_pages = total_pages
 
     def validate(self):
         if self.content:
             self.content.validate()
@@ -2103,30 +2110,30 @@
         data: DescribeDownloadTaskResponseBodyData = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code.
+        # The error code returned if the request fails.
         self.code = code
-        # The details of the download tasks.
+        # The details of the download task.
         self.data = data
-        # The error code.
+        # The error code returned if the request fails.
         self.err_code = err_code
-        # The error message.
+        # The error message returned if the request fails.
         self.err_message = err_message
-        # The error message.
+        # The error message returned if the request fails.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful. Valid values:
+        # Indicates whether the request was successful. Valid values:
         # 
-        # *   **true**: The request is successful.
-        # *   **false**: The request fails.
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -2219,27 +2226,27 @@
     def __init__(
         self,
         backup_plan_id: str = None,
         backup_set_id: str = None,
         page_number: str = None,
         page_size: str = None,
     ):
-        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to obtain the ID of the backup schedule.
+        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to query the ID of the backup schedule.
         # 
-        # >  If your instance is an ApsaraDB RDS for MySQL instance, you can configure [automatic access to the instance](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
         self.backup_plan_id = backup_plan_id
-        # The ID of the backup set. If this parameter is specified, only the snapshot of the backup set is returned. If this parameter is not specified, all the snapshots of the backup schedule are returned.
+        # The ID of the backup set. If this parameter is specified, only the snapshot of the specified backup set is returned. If this parameter is not specified, all the snapshots of the backup schedule are returned.
         self.backup_set_id = backup_set_id
-        # The number of the page to return. The value must be an integer that is greater than 0. Default value: 1.
+        # The number of the page to return. Pages start from page 1. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values:
         # 
-        # *   30 (default value)
-        # *   50
-        # *   100
+        # *   30: This is the default value.
+        # *   50\.
+        # *   100\.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2277,32 +2284,32 @@
         data: str = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code.
+        # The error code returned if the request failed.
         self.code = code
-        # The response parameters.
+        # The returned data. The following parameters are contained:
         # 
         # *   **backupSetTime**: the point in time when the snapshot was created. The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mm:ssZ format. The time is displayed in UTC.
         # *   **backupSetId**: the ID of the backup set.
         # *   **backupSetType**: the type of the snapshot. A value of **Full** indicates that the snapshot is a full backup snapshot. A value of **Inc** indicates that the snapshot is an incremental backup snapshot.
         # *   **backupPlanId**: the ID of the backup schedule.
         self.data = data
-        # The error code.
+        # The error code returned if the request failed.
         self.err_code = err_code
-        # The error message.
+        # The error message returned if the request failed.
         self.err_message = err_message
-        # The error message.
+        # The error message returned if the request failed.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful.
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2395,23 +2402,23 @@
         backup_plan_id: str = None,
         instance_id: str = None,
         page_number: str = None,
         page_size: str = None,
     ):
         # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to obtain the ID of the backup schedule.
         # 
-        # >  If your instance is an ApsaraDB RDS for MySQL instance, you can configure [automatic access to the instance](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
         self.backup_plan_id = backup_plan_id
-        # The ID of the sandbox instance. You can call the [CreateSandboxInstance](~~437252~~) parameter to obtain the ID of the sandbox instance.
+        # The ID of the sandbox instance. You can call the [CreateSandboxInstance](~~437252~~) operation to obtain the ID of the sandbox instance.
         self.instance_id = instance_id
         # The number of the page to return. The value must be an integer that is greater than 0. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values:
         # 
-        # *   30 (default value)
+        # *   30\. This is the default value.
         # *   50
         # *   100
         self.page_size = page_size
 
     def validate(self):
         pass
 
@@ -2451,15 +2458,15 @@
         data: str = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code.
+        # The error code returned if the request fails.
         self.code = code
         # The response parameters.
         # 
         # *   **connectionString**: the connection string of the sandbox instance, in the format of IP address:Port number. This parameter indicates the endpoint of the sandbox instance if the value of the SandboxType parameter is **Sandbox**. This parameter indicates the Network File System (NFS) mount address if the value of the SandboxType parameter is **NFS**.
         # *   **restoreSeconds**: the time required to create the sandbox instance. Unit: seconds.
         # *   **restoreTime**: the point in time to which the sandbox instance is restored. The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mm:ssZ format. The time is displayed in UTC.
         # *   **instanceId**: the ID of the sandbox instance.
@@ -2467,23 +2474,23 @@
         # *   **createTime**: the point in time when the sandbox instance was created. The time follows the ISO 8601 standard in the yyyy-MM-ddThh:mm:ssZ format. The time is displayed in UTC.
         # *   **backupPlanId**: the ID of the backup schedule.
         # *   **vpcId**: the ID of the virtual private cloud (VPC).
         # *   **vpcSwitchId**: the ID of the VSwitch.
         # *   **sandboxSpecification**: the specifications of the sandbox instance.
         # *   **status**: the status of the sandbox instance. Valid values: **running**, **check_pass**, and **stop**.
         self.data = data
-        # The error code.
+        # The error code returned if the request fails.
         self.err_code = err_code
-        # The error message.
+        # The error message returned if the request fails.
         self.err_message = err_message
-        # The error message.
+        # The error message returned if the request fails.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful.
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2573,15 +2580,15 @@
 class DescribeSandboxRecoveryTimeRequest(TeaModel):
     def __init__(
         self,
         backup_plan_id: str = None,
     ):
         # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to obtain the ID of the backup schedule. If you set this parameter to the backup schedule ID obtained by calling the DescribeBackupPlanList operation, the dbs prefix must be removed. Otherwise, the call fails.
         # 
-        # >  If your instance is an ApsaraDB RDS for MySQL instance, you can configure [automatic access to the instance](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
         self.backup_plan_id = backup_plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2649,27 +2656,27 @@
         data: DescribeSandboxRecoveryTimeResponseBodyData = None,
         err_code: str = None,
         err_message: str = None,
         message: str = None,
         request_id: str = None,
         success: str = None,
     ):
-        # The error code.
+        # The error code returned if the request fails.
         self.code = code
         # The response parameters.
         self.data = data
-        # The error code.
+        # The error code returned if the request fails.
         self.err_code = err_code
-        # The error message.
+        # The error message returned if the request fails.
         self.err_message = err_message
-        # The error message.
+        # The error message returned if the request fails.
         self.message = message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful.
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -2760,21 +2767,19 @@
 
 class ModifyDBTablesRecoveryStateRequest(TeaModel):
     def __init__(
         self,
         category: str = None,
         instance_id: str = None,
         region_code: str = None,
-        region_id: str = None,
         retention: str = None,
     ):
         self.category = category
         self.instance_id = instance_id
         self.region_code = region_code
-        self.region_id = region_id
         self.retention = retention
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2784,30 +2789,26 @@
         result = dict()
         if self.category is not None:
             result['Category'] = self.category
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.region_code is not None:
             result['RegionCode'] = self.region_code
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
         if self.retention is not None:
             result['Retention'] = self.retention
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Category') is not None:
             self.category = m.get('Category')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionCode') is not None:
             self.region_code = m.get('RegionCode')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
         if m.get('Retention') is not None:
             self.retention = m.get('Retention')
         return self
 
 
 class ModifyDBTablesRecoveryStateResponseBody(TeaModel):
     def __init__(
@@ -2917,45 +2918,39 @@
 
 
 class SupportDBTableRecoveryRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_code: str = None,
-        region_id: str = None,
     ):
         self.instance_id = instance_id
         self.region_code = region_code
-        self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.region_code is not None:
             result['RegionCode'] = self.region_code
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionCode') is not None:
             self.region_code = m.get('RegionCode')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
         return self
 
 
 class SupportDBTableRecoveryResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
```

### Comparing `alibabacloud_dbs20210101-1.0.2/alibabacloud_dbs20210101.egg-info/PKG-INFO` & `alibabacloud_dbs20210101-1.0.3/alibabacloud_dbs20210101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dbs20210101
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Dbs (20210101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dbs20210101-1.0.2/setup.py` & `alibabacloud_dbs20210101-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dbs20210101.
 
-Created on 31/01/2023
+Created on 26/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dbs20210101"
 NAME = "alibabacloud_dbs20210101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dbs (20210101) SDK Library for Python"
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

