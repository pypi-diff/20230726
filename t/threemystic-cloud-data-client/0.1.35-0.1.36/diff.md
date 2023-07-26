# Comparing `tmp/threemystic_cloud_data_client-0.1.35.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.36.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.35.tar` & `threemystic_cloud_data_client-0.1.36.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0    17963 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/hatch.toml
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/pyproject.toml
--rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.35/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmss.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11867 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    13572 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    22664 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/hatch.toml
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/pyproject.toml
+-rw-r--r--   0        0        0     4677 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.36/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The AWS vm Action. This will pull the AWS EC2s"""
 from threemystic_cloud_data_client.cloud_providers.aws.client.actions.base_class.base import cloud_data_client_aws_client_action_base as base
 import asyncio
 from threemystic_cloud_data_client.cloud_providers.aws.client.actions.vmimage import cloud_data_client_aws_client_action as vmimage_data
 
 class cloud_data_client_aws_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
@@ -32,15 +33,15 @@
     self.required_extra_data["instances_information"] = {}
     if self.required_extra_data.get("ami") is None:
       base_action_params = {
         "cloud_data_client": self._get_cloud_data_client_raw(),
         "common": self.get_common(),
         "logger": self.get_common().get_logger()
       }
-      # This is required because #the normal disk command only looks at long lived disks
+      
       ami_data = vmimage_data(
         **base_action_params
       )
       tmp_ami_data = await ami_data.main(pool=pool, run_params= self.get_runparam_key(data_key= None))
       self.required_extra_data["ami"] = await ami_data.get_data_by_id(results= tmp_ami_data, id_override = "extra_id_only")
 
   def _process_preloaded_data(self, preloaded_data = None, *args, **kwargs):
@@ -183,25 +184,25 @@
         boto_params={},
         boto_nextkey = "NextToken",
         boto_key="Volumes"
       )
 
       return { data["VolumeId"]:data for data in volumne_data }
   
-  async def __getImageInfo(self, imageId):
-    if imageId in self.required_extra_data["ami"]:
+  async def __getImageInfo(self, image_id, *args, **kwargs):
+    if image_id in self.required_extra_data["ami"]:
       return {
-        "Id": imageId,
-        "Name": self.required_extra_data["ami"][imageId]["Name"],
+        "Id": image_id,
+        "Name": self.required_extra_data["ami"][image_id]["Name"],
         "Description": self.required_extra_data["ami"].get("Description")
       }
 
 
     return {
-      "Id": imageId,
+      "Id": image_id,
     }
   
   async def __get_instance_attribute(self, client, instance, loop, attribute = None, *args, **kwargs):
     # Full attribute list
     # 'instanceType','kernel','ramdisk','userData','disableApiTermination','instanceInitiatedShutdownBehavior','rootDeviceName','blockDeviceMapping','productCodes','sourceDestCheck','groupSet','ebsOptimized','sriovNetSupport','enaSupport','enclaveOptions','disableApiStop'
     # to use groupSet you need to specify an interface ID when multiple interfaces are attached
 
@@ -283,15 +284,15 @@
         "Version": instance_information.get('AgentVersion'),
     } 
   
   async def __get_instance_withextra_data(self, ec2_client, ssm_client, task_asg_by_instance, account, region, lb_instances, instance, loop, *args, **kwargs):
       
       
       extra_data_tasks = {
-        "extra_image": loop.create_task(self.__getImageInfo(imageId= instance["ImageId"])),
+        "extra_image": loop.create_task(self.__getImageInfo(image_id= instance["ImageId"])),
         "extra_instance_attributes": loop.create_task(self.__get_instance_attribute(account=account, client= ec2_client, instance=instance, loop= loop)),
         "extra_ssminfo": loop.create_task(self.__getSSMInfo(account=account, region=region, ssm_client=ssm_client, instance=instance)),
         "_ignore_extra_asg": task_asg_by_instance
         
       }      
 
       extra_data = {
```

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The AWS VMImage Action. This will pull the AWS AMIs"""
 from threemystic_cloud_data_client.cloud_providers.aws.client.actions.base_class.base import cloud_data_client_aws_client_action_base as base
 import asyncio
 
 
 class cloud_data_client_aws_client_action(base):
   def __init__(self, *args, **kwargs):
     super().__init__(
```

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.36/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/.gitignore` & `threemystic_cloud_data_client-0.1.36/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/LICENSE` & `threemystic_cloud_data_client-0.1.36/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/README.md` & `threemystic_cloud_data_client-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/hatch.toml` & `threemystic_cloud_data_client-0.1.36/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/pyproject.toml` & `threemystic_cloud_data_client-0.1.36/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.35/PKG-INFO` & `threemystic_cloud_data_client-0.1.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.35
+Version: 0.1.36
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

