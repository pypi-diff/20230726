# Comparing `tmp/threemystic_cloud_client-0.1.49.tar.gz` & `tmp/threemystic_cloud_client-0.1.50.tar.gz`

## Comparing `threemystic_cloud_client-0.1.49.tar` & `threemystic_cloud_client-0.1.50.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/actions/action_generate/__init__.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/actions/action_test/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/actions/action_token/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
--rw-r--r--   0        0        0    34170 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
--rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    17146 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/LICENSE
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/hatch.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/pyproject.toml
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.49/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/actions/action_generate/__init__.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/actions/action_test/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/actions/action_token/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     6289 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py
+-rw-r--r--   0        0        0    34457 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12277 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py
+-rw-r--r--   0        0        0    15659 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/LICENSE
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/hatch.toml
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/pyproject.toml
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.50/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/actions/action_generate/__init__.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/actions/action_generate/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/actions/action_test/__init__.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/actions/action_test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/actions/action_token/__init__.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/actions/action_token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_generate/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_generate/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -764,18 +764,23 @@
   
   def get_resource_tags_as_dictionary(self, resource, *args, **kwargs):
     if resource is None:
       return None
 
     tags = None
     if not self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
+      if hasattr(resource, "extra_tags"):
+        if resource.extra_tags is not None and len(resource.extra_tags) > 0:
+          return resource.extra_tags
       if hasattr(resource, "tags"):
         tags = resource.tags
         
     elif self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
+      if resource.get("extra_tags") is not None and len(resource.get("extra_tags")) > 0:
+        return resource.get("extra_tags")
       tags = resource.get("tags")
 
     if tags is None:
       tags = {}
     
     if self.get_common().helper_type().general().is_type(obj= tags, type_check= list ):
         tags = {tag["Key"]:tag["Value"] for tag in tags}
```

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/action_test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/action_test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/action_token/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/action_token/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -331,17 +331,23 @@
   
   def get_resource_tags_as_dictionary(self, resource, *args, **kwargs):
     if resource is None:
       return None
 
     tags = None
     if not self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
+      if hasattr(resource, "extra_tags"):
+        if resource.extra_tags is not None and len(resource.extra_tags) > 0:
+          return resource.extra_tags
+        
       if hasattr(resource, "tags"):
         tags = resource.tags
     elif self.get_common().helper_type().general().is_type(obj= resource, type_check= dict):
+      if resource.get("extra_tags") is not None and len(resource.get("extra_tags")) > 0:
+        return resource.get("extra_tags")
       tags = resource.get("tags")
 
     if tags is None:
       tags = {}
       
     if "name" not in tags:
       name_options = ["display_name", "displayname", "name"]
```

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.50/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/.gitignore` & `threemystic_cloud_client-0.1.50/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/LICENSE` & `threemystic_cloud_client-0.1.50/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/README.md` & `threemystic_cloud_client-0.1.50/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/hatch.toml` & `threemystic_cloud_client-0.1.50/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/pyproject.toml` & `threemystic_cloud_client-0.1.50/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.49/PKG-INFO` & `threemystic_cloud_client-0.1.50/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.49
+Version: 0.1.50
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

