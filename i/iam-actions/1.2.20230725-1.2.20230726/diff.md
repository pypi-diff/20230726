# Comparing `tmp/iam_actions-1.2.20230725.tar.gz` & `tmp/iam_actions-1.2.20230726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230725.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230726.tar", max compression
```

## Comparing `iam_actions-1.2.20230725.tar` & `iam_actions-1.2.20230726.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/LICENSE
--rw-r--r--   0        0        0     2302 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/README.md
--rw-r--r--   0        0        0      228 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/__init__.py
--rw-r--r--   0        0        0  4375008 2023-07-25 02:42:07.572322 iam_actions-1.2.20230725/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-07-25 02:40:43.508074 iam_actions-1.2.20230725/iam_actions/generate/services.py
--rw-r--r--   0        0        0   563046 2023-07-25 02:42:07.572322 iam_actions-1.2.20230725/iam_actions/policies.json
--rw-r--r--   0        0        0   197464 2023-07-25 02:42:07.572322 iam_actions-1.2.20230725/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   546095 2023-07-25 02:42:07.572322 iam_actions-1.2.20230725/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-07-25 02:42:08.340324 iam_actions-1.2.20230725/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230725/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230725/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/LICENSE
+-rw-r--r--   0        0        0     2302 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/README.md
+-rw-r--r--   0        0        0      228 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4377792 2023-07-26 02:33:43.655265 iam_actions-1.2.20230726/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-07-26 02:31:33.489491 iam_actions-1.2.20230726/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-07-26 02:31:33.493491 iam_actions-1.2.20230726/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-07-26 02:31:33.493491 iam_actions-1.2.20230726/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-07-26 02:31:33.493491 iam_actions-1.2.20230726/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   563521 2023-07-26 02:33:43.655265 iam_actions-1.2.20230726/iam_actions/policies.json
+-rw-r--r--   0        0        0   197464 2023-07-26 02:33:43.655265 iam_actions-1.2.20230726/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   546555 2023-07-26 02:33:43.655265 iam_actions-1.2.20230726/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-07-26 02:33:44.615337 iam_actions-1.2.20230726/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230726/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230726/PKG-INFO
```

### Comparing `iam_actions-1.2.20230725/LICENSE` & `iam_actions-1.2.20230726/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230725/README.md` & `iam_actions-1.2.20230726/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230725/iam_actions/actions.json` & `iam_actions-1.2.20230726/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997278031883121%*

 * *Differences: {"'profile'": "{'GetSimilarProfiles': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *              "'GetSimilarProfiles'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *              "AWS'), ('orphan', False), ('resources', [])]), 'ListRuleBasedMatches': "*

 * *              "OrderedDict([('access_level', 'Undocumented'), ('action', 'ListRuleBasedMatches'), "*

 * *              "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', "*

 * *              "False), ('resource […]*

```diff
@@ -109841,14 +109841,22 @@
             "access_level": "Read",
             "action": "GetProfileObjectTypeTemplate",
             "condition_keys": [],
             "description": "Grants permission to get a specific object type template",
             "orphan": false,
             "resources": []
         },
+        "GetSimilarProfiles": {
+            "access_level": "Undocumented",
+            "action": "GetSimilarProfiles",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetWorkflow": {
             "access_level": "Read",
             "action": "GetWorkflow",
             "condition_keys": [],
             "description": "Grants permission to get workflow details in a domain",
             "orphan": false,
             "resources": [
@@ -109956,14 +109964,22 @@
             "description": "Grants permission to list all the profile objects for a profile",
             "orphan": false,
             "resources": [
                 "domains",
                 "object-types"
             ]
         },
+        "ListRuleBasedMatches": {
+            "access_level": "Undocumented",
+            "action": "ListRuleBasedMatches",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags for a resource",
             "orphan": false,
             "resources": [
@@ -112464,14 +112480,30 @@
             "condition_keys": [],
             "description": "Grants permission to describe permissions for a QuickSight Dashboard",
             "orphan": false,
             "resources": [
                 "dashboard"
             ]
         },
+        "DescribeDashboardSnapshotJob": {
+            "access_level": "Undocumented",
+            "action": "DescribeDashboardSnapshotJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeDashboardSnapshotJobResult": {
+            "access_level": "Undocumented",
+            "action": "DescribeDashboardSnapshotJobResult",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeDataSet": {
             "access_level": "Read",
             "action": "DescribeDataSet",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -113302,14 +113334,22 @@
             "condition_keys": [],
             "description": "Grants permission to search for a sub-set of QuickSight groups",
             "orphan": false,
             "resources": [
                 "group"
             ]
         },
+        "SearchUsers": {
+            "access_level": "Undocumented",
+            "action": "SearchUsers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "SetGroupMapping": {
             "access_level": "Write",
             "action": "SetGroupMapping",
             "condition_keys": [],
             "description": "Grants permission to use Amazon QuickSight, in Enterprise edition, to display your Microsoft Active Directory directory groups so that you can choose which ones to map to roles in Amazon QuickSight",
             "orphan": false,
             "resources": []
@@ -113330,14 +113370,22 @@
             "condition_keys": [],
             "description": "Grants permission to start an asset bundle import job",
             "orphan": false,
             "resources": [
                 "assetBundleImportJob"
             ]
         },
+        "StartDashboardSnapshotJob": {
+            "access_level": "Undocumented",
+            "action": "StartDashboardSnapshotJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "Subscribe": {
             "access_level": "Write",
             "action": "Subscribe",
             "condition_keys": [
                 "quicksight:DirectoryType",
                 "quicksight:Edition"
             ],
@@ -122327,14 +122375,22 @@
             ],
             "description": "Grants permission to create a Firewall rule group",
             "orphan": false,
             "resources": [
                 "firewall-rule-group"
             ]
         },
+        "CreateOutpostResolver": {
+            "access_level": "Undocumented",
+            "action": "CreateOutpostResolver",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateResolverEndpoint": {
             "access_level": "Write",
             "action": "CreateResolverEndpoint",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -122395,14 +122451,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete a Firewall rule group",
             "orphan": false,
             "resources": [
                 "firewall-rule-group"
             ]
         },
+        "DeleteOutpostResolver": {
+            "access_level": "Undocumented",
+            "action": "DeleteOutpostResolver",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteResolverEndpoint": {
             "access_level": "Write",
             "action": "DeleteResolverEndpoint",
             "condition_keys": [],
             "description": "Grants permission to delete a Resolver endpoint. The effect of deleting a Resolver endpoint depends on whether it's an inbound or an outbound endpoint",
             "orphan": false,
             "resources": [
@@ -122515,14 +122579,22 @@
             "condition_keys": [],
             "description": "Grants permission to get information about a specified Firewall rule group policy, which specifies the Firewall rule group operations and resources that you want to allow another AWS account to use",
             "orphan": false,
             "resources": [
                 "firewall-rule-group"
             ]
         },
+        "GetOutpostResolver": {
+            "access_level": "Undocumented",
+            "action": "GetOutpostResolver",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetResolverConfig": {
             "access_level": "Read",
             "action": "GetResolverConfig",
             "condition_keys": [],
             "description": "Grants permission to get the Resolver Config status within the specified resource",
             "orphan": false,
             "resources": [
@@ -122665,14 +122737,22 @@
             "condition_keys": [],
             "description": "Grants permission to list all the Firewall rule under a speicfied Firewall rule group",
             "orphan": false,
             "resources": [
                 "firewall-rule-group"
             ]
         },
+        "ListOutpostResolvers": {
+            "access_level": "Undocumented",
+            "action": "ListOutpostResolvers",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListResolverConfigs": {
             "access_level": "List",
             "action": "ListResolverConfigs",
             "condition_keys": [],
             "description": "Grants permission to list Resolver Config statuses",
             "orphan": false,
             "resources": [
@@ -122860,14 +122940,22 @@
             "condition_keys": [],
             "description": "Grants permission to update selected settings for an Firewall rule group association",
             "orphan": false,
             "resources": [
                 "firewall-rule-group-association"
             ]
         },
+        "UpdateOutpostResolver": {
+            "access_level": "Undocumented",
+            "action": "UpdateOutpostResolver",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateResolverConfig": {
             "access_level": "Write",
             "action": "UpdateResolverConfig",
             "condition_keys": [],
             "description": "Grants permission to update the Resolver Config status within the specified resource",
             "orphan": false,
             "resources": [
@@ -142082,14 +142170,22 @@
             "access_level": "Write",
             "action": "RestoreDatabase",
             "condition_keys": [],
             "description": "Grants permission to restore a database from another database",
             "orphan": false,
             "resources": []
         },
+        "StartApplicationRefresh": {
+            "access_level": "Undocumented",
+            "action": "StartApplicationRefresh",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -147943,14 +148039,22 @@
                 "host-key",
                 "profile",
                 "server",
                 "user",
                 "workflow"
             ]
         },
+        "TestConnection": {
+            "access_level": "Undocumented",
+            "action": "TestConnection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TestIdentityProvider": {
             "access_level": "Read",
             "action": "TestIdentityProvider",
             "condition_keys": [],
             "description": "Grants permission to test a server's custom identity provider",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20230725/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230726/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230725/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230726/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230725/iam_actions/generate/generate.py` & `iam_actions-1.2.20230726/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230725/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230726/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230725/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230726/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230725/iam_actions/generate/services.py` & `iam_actions-1.2.20230726/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230725/iam_actions/policies.json` & `iam_actions-1.2.20230726/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989545079228908%*

 * *Differences: {"'serviceMap'": "{'AWS Systems Manager': {'conditionKeys': {insert: [(10, "*

 * *                 "'ssm:resourceTag/aws:ssmmessages:session-id'), (11, "*

 * *                 "'ssm:resourceTag/aws:ssmmessages:target-id')]}}, 'Amazon Connect Customer "*

 * *                 "Profiles': {'Actions': {insert: [(25, 'GetSimilarProfiles'), (38, "*

 * *                 "'ListRuleBasedMatches')]}}, 'Amazon Route 53 Resolver': {'Actions': {insert: "*

 * *                 "[(7, 'CreateOutpostResolver'), (14, 'DeleteOutpostResolver'), (27, " […]*

```diff
@@ -4489,14 +4489,136 @@
             "StringPrefix": "medical-imaging",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "AWS HealthLake": {
+            "ARNFormat": "arn:aws:healthlake:${Region}:${Account}:${ResourceType}/${ResourceName}",
+            "ARNRegex": "^arn:aws:healthlake:.+:.+:.+",
+            "Actions": [
+                "CreateFHIRDatastore",
+                "CreateResource",
+                "DeleteFHIRDatastore",
+                "DeleteResource",
+                "DescribeFHIRDatastore",
+                "DescribeFHIRExportJob",
+                "DescribeFHIRImportJob",
+                "GetCapabilities",
+                "ListFHIRDatastores",
+                "ListFHIRExportJobs",
+                "ListFHIRImportJobs",
+                "ListTagsForResource",
+                "ReadResource",
+                "SearchWithGet",
+                "SearchWithPost",
+                "StartFHIRExportJob",
+                "StartFHIRImportJob",
+                "TagResource",
+                "UntagResource",
+                "UpdateResource"
+            ],
+            "HasResource": true,
+            "StringPrefix": "healthlake",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
+        "AWS HealthOmics": {
+            "ARNFormat": "arn:aws:omics:${Region}:${Account}:${ResourceType}/${ResourcePath}",
+            "ARNRegex": "^arn:aws:omics:${Region}:${Account}?:${ResourceType}/.+?",
+            "Actions": [
+                "AbortMultipartReadSetUpload",
+                "BatchDeleteReadSet",
+                "CancelAnnotationImportJob",
+                "CancelRun",
+                "CancelVariantImportJob",
+                "CompleteMultipartReadSetUpload",
+                "CreateAnnotationStore",
+                "CreateMultipartReadSetUpload",
+                "CreateReferenceStore",
+                "CreateRunGroup",
+                "CreateSequenceStore",
+                "CreateVariantStore",
+                "CreateWorkflow",
+                "DeleteAnnotationStore",
+                "DeleteReference",
+                "DeleteReferenceStore",
+                "DeleteRun",
+                "DeleteRunGroup",
+                "DeleteSequenceStore",
+                "DeleteVariantStore",
+                "DeleteWorkflow",
+                "GetAnnotationImportJob",
+                "GetAnnotationStore",
+                "GetReadSet",
+                "GetReadSetActivationJob",
+                "GetReadSetExportJob",
+                "GetReadSetImportJob",
+                "GetReadSetMetadata",
+                "GetReference",
+                "GetReferenceImportJob",
+                "GetReferenceMetadata",
+                "GetReferenceStore",
+                "GetRun",
+                "GetRunGroup",
+                "GetRunTask",
+                "GetSequenceStore",
+                "GetVariantImportJob",
+                "GetVariantStore",
+                "GetWorkflow",
+                "ListAnnotationImportJobs",
+                "ListAnnotationStores",
+                "ListMultipartReadSetUploads",
+                "ListReadSetActivationJobs",
+                "ListReadSetExportJobs",
+                "ListReadSetImportJobs",
+                "ListReadSetUploadParts",
+                "ListReadSets",
+                "ListReferenceImportJobs",
+                "ListReferenceStores",
+                "ListReferences",
+                "ListRunGroups",
+                "ListRunTasks",
+                "ListRuns",
+                "ListSequenceStores",
+                "ListTagsForResource",
+                "ListVariantImportJobs",
+                "ListVariantStores",
+                "ListWorkflows",
+                "StartAnnotationImportJob",
+                "StartReadSetActivationJob",
+                "StartReadSetExportJob",
+                "StartReadSetImportJob",
+                "StartReferenceImportJob",
+                "StartRun",
+                "StartVariantImportJob",
+                "TagResource",
+                "UntagResource",
+                "UpdateAnnotationStore",
+                "UpdateRunGroup",
+                "UpdateVariantStore",
+                "UpdateWorkflow",
+                "UploadReadSetPart"
+            ],
+            "HasResource": true,
+            "StringPrefix": "omics",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "omics:AnnotationImportJobJobId",
+                "omics:AnnotationStoreName",
+                "omics:VariantImportJobJobId",
+                "omics:VariantStoreName"
+            ]
+        },
         "AWS IAM Access Analyzer": {
             "ARNFormat": "arn:aws:access-analyzer:${Region}:${Account}:analyzer/${AnalyzerName}",
             "ARNRegex": "^arn:aws:access-analyzer:.+",
             "Actions": [
                 "ApplyArchiveRule",
                 "CancelPolicyGeneration",
                 "CreateAccessPreview",
@@ -8982,14 +9104,16 @@
                 "ssm:AutoApprove",
                 "ssm:DocumentCategories",
                 "ssm:Overwrite",
                 "ssm:Recursive",
                 "ssm:SessionDocumentAccessCheck",
                 "ssm:SyncType",
                 "ssm:resourceTag/${TagKey}",
+                "ssm:resourceTag/aws:ssmmessages:session-id",
+                "ssm:resourceTag/aws:ssmmessages:target-id",
                 "ssm:resourceTag/tag-key"
             ]
         },
         "AWS Systems Manager GUI Connect": {
             "Actions": [
                 "CancelConnection",
                 "GetConnection",
@@ -9109,14 +9233,15 @@
                 "ListComponents",
                 "ListDatabases",
                 "ListOperations",
                 "ListTagsForResource",
                 "PutResourcePermission",
                 "RegisterApplication",
                 "RestoreDatabase",
+                "StartApplicationRefresh",
                 "TagResource",
                 "UntagResource",
                 "UpdateApplicationSettings",
                 "UpdateHANABackupSettings"
             ],
             "HasResource": true,
             "StringPrefix": "ssm-sap",
@@ -9262,14 +9387,15 @@
                 "ListUsers",
                 "ListWorkflows",
                 "SendWorkflowStepState",
                 "StartFileTransfer",
                 "StartServer",
                 "StopServer",
                 "TagResource",
+                "TestConnection",
                 "TestIdentityProvider",
                 "UntagResource",
                 "UpdateAccess",
                 "UpdateAgreement",
                 "UpdateCertificate",
                 "UpdateConnector",
                 "UpdateHostKey",
@@ -11961,26 +12087,28 @@
                 "GetDomain",
                 "GetEventStream",
                 "GetIdentityResolutionJob",
                 "GetIntegration",
                 "GetMatches",
                 "GetProfileObjectType",
                 "GetProfileObjectTypeTemplate",
+                "GetSimilarProfiles",
                 "GetWorkflow",
                 "GetWorkflowSteps",
                 "ListAccountIntegrations",
                 "ListCalculatedAttributeDefinitions",
                 "ListCalculatedAttributesForProfile",
                 "ListDomains",
                 "ListEventStreams",
                 "ListIdentityResolutionJobs",
                 "ListIntegrations",
                 "ListProfileObjectTypeTemplates",
                 "ListProfileObjectTypes",
                 "ListProfileObjects",
+                "ListRuleBasedMatches",
                 "ListTagsForResource",
                 "ListWorkflows",
                 "MergeProfiles",
                 "PutIntegration",
                 "PutProfileObject",
                 "PutProfileObjectType",
                 "SearchProfiles",
@@ -14665,47 +14793,14 @@
             "StringPrefix": "guardduty",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
-        "Amazon HealthLake": {
-            "ARNFormat": "arn:aws:healthlake:${Region}:${AccountId}:${ResourceType}/${ResourceName}",
-            "ARNRegex": "^arn:aws:healthlake:.+:.+:.+",
-            "Actions": [
-                "CreateFHIRDatastore",
-                "CreateResource",
-                "DeleteFHIRDatastore",
-                "DeleteResource",
-                "DescribeFHIRDatastore",
-                "DescribeFHIRExportJob",
-                "DescribeFHIRImportJob",
-                "GetCapabilities",
-                "ListFHIRDatastores",
-                "ListFHIRExportJobs",
-                "ListFHIRImportJobs",
-                "ListTagsForResource",
-                "ReadResource",
-                "SearchWithGet",
-                "SearchWithPost",
-                "StartFHIRExportJob",
-                "StartFHIRImportJob",
-                "TagResource",
-                "UntagResource",
-                "UpdateResource"
-            ],
-            "HasResource": true,
-            "StringPrefix": "healthlake",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
-            ]
-        },
         "Amazon Honeycode": {
             "ARNFormat": "arn:aws:honeycode:${Region}:${Account}:${ResourceType}:${ResourcePath}",
             "ARNRegex": "^arn:aws:honeycode:.+:.+:.+",
             "Actions": [
                 "ApproveTeamAssociation",
                 "BatchCreateTableRows",
                 "BatchDeleteTableRows",
@@ -16440,103 +16535,14 @@
                 "nimble:createdBy",
                 "nimble:ownedBy",
                 "nimble:principalId",
                 "nimble:requesterPrincipalId",
                 "nimble:studioId"
             ]
         },
-        "Amazon Omics": {
-            "ARNFormat": "arn:aws:omics:${Region}:${Account}:${ResourceType}/${ResourcePath}",
-            "ARNRegex": "^arn:aws:omics:${Region}:${Account}?:${ResourceType}/.+?",
-            "Actions": [
-                "AbortMultipartReadSetUpload",
-                "BatchDeleteReadSet",
-                "CancelAnnotationImportJob",
-                "CancelRun",
-                "CancelVariantImportJob",
-                "CompleteMultipartReadSetUpload",
-                "CreateAnnotationStore",
-                "CreateMultipartReadSetUpload",
-                "CreateReferenceStore",
-                "CreateRunGroup",
-                "CreateSequenceStore",
-                "CreateVariantStore",
-                "CreateWorkflow",
-                "DeleteAnnotationStore",
-                "DeleteReference",
-                "DeleteReferenceStore",
-                "DeleteRun",
-                "DeleteRunGroup",
-                "DeleteSequenceStore",
-                "DeleteVariantStore",
-                "DeleteWorkflow",
-                "GetAnnotationImportJob",
-                "GetAnnotationStore",
-                "GetReadSet",
-                "GetReadSetActivationJob",
-                "GetReadSetExportJob",
-                "GetReadSetImportJob",
-                "GetReadSetMetadata",
-                "GetReference",
-                "GetReferenceImportJob",
-                "GetReferenceMetadata",
-                "GetReferenceStore",
-                "GetRun",
-                "GetRunGroup",
-                "GetRunTask",
-                "GetSequenceStore",
-                "GetVariantImportJob",
-                "GetVariantStore",
-                "GetWorkflow",
-                "ListAnnotationImportJobs",
-                "ListAnnotationStores",
-                "ListMultipartReadSetUploads",
-                "ListReadSetActivationJobs",
-                "ListReadSetExportJobs",
-                "ListReadSetImportJobs",
-                "ListReadSetUploadParts",
-                "ListReadSets",
-                "ListReferenceImportJobs",
-                "ListReferenceStores",
-                "ListReferences",
-                "ListRunGroups",
-                "ListRunTasks",
-                "ListRuns",
-                "ListSequenceStores",
-                "ListTagsForResource",
-                "ListVariantImportJobs",
-                "ListVariantStores",
-                "ListWorkflows",
-                "StartAnnotationImportJob",
-                "StartReadSetActivationJob",
-                "StartReadSetExportJob",
-                "StartReadSetImportJob",
-                "StartReferenceImportJob",
-                "StartRun",
-                "StartVariantImportJob",
-                "TagResource",
-                "UntagResource",
-                "UpdateAnnotationStore",
-                "UpdateRunGroup",
-                "UpdateVariantStore",
-                "UpdateWorkflow",
-                "UploadReadSetPart"
-            ],
-            "HasResource": true,
-            "StringPrefix": "omics",
-            "conditionKeys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys",
-                "omics:AnnotationImportJobJobId",
-                "omics:AnnotationStoreName",
-                "omics:VariantImportJobJobId",
-                "omics:VariantStoreName"
-            ]
-        },
         "Amazon OpenSearch Ingestion": {
             "ARNFormat": "arn:aws:osis:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:osis:.+:.+:.+",
             "Actions": [
                 "CreatePipeline",
                 "DeletePipeline",
                 "GetPipeline",
@@ -17188,14 +17194,16 @@
                 "DescribeAnalysis",
                 "DescribeAnalysisPermissions",
                 "DescribeAssetBundleExportJob",
                 "DescribeAssetBundleImportJob",
                 "DescribeCustomPermissions",
                 "DescribeDashboard",
                 "DescribeDashboardPermissions",
+                "DescribeDashboardSnapshotJob",
+                "DescribeDashboardSnapshotJobResult",
                 "DescribeDataSet",
                 "DescribeDataSetPermissions",
                 "DescribeDataSetRefreshProperties",
                 "DescribeDataSource",
                 "DescribeDataSourcePermissions",
                 "DescribeEmailCustomizationTemplate",
                 "DescribeFolder",
@@ -17269,17 +17277,19 @@
                 "SearchAnalyses",
                 "SearchDashboards",
                 "SearchDataSets",
                 "SearchDataSources",
                 "SearchDirectoryGroups",
                 "SearchFolders",
                 "SearchGroups",
+                "SearchUsers",
                 "SetGroupMapping",
                 "StartAssetBundleExportJob",
                 "StartAssetBundleImportJob",
+                "StartDashboardSnapshotJob",
                 "Subscribe",
                 "TagResource",
                 "Unsubscribe",
                 "UntagResource",
                 "UpdateAccountCustomization",
                 "UpdateAccountSettings",
                 "UpdateAnalysis",
@@ -18131,32 +18141,35 @@
                 "AssociateFirewallRuleGroup",
                 "AssociateResolverEndpointIpAddress",
                 "AssociateResolverQueryLogConfig",
                 "AssociateResolverRule",
                 "CreateFirewallDomainList",
                 "CreateFirewallRule",
                 "CreateFirewallRuleGroup",
+                "CreateOutpostResolver",
                 "CreateResolverEndpoint",
                 "CreateResolverQueryLogConfig",
                 "CreateResolverRule",
                 "DeleteFirewallDomainList",
                 "DeleteFirewallRule",
                 "DeleteFirewallRuleGroup",
+                "DeleteOutpostResolver",
                 "DeleteResolverEndpoint",
                 "DeleteResolverQueryLogConfig",
                 "DeleteResolverRule",
                 "DisassociateFirewallRuleGroup",
                 "DisassociateResolverEndpointIpAddress",
                 "DisassociateResolverQueryLogConfig",
                 "DisassociateResolverRule",
                 "GetFirewallConfig",
                 "GetFirewallDomainList",
                 "GetFirewallRuleGroup",
                 "GetFirewallRuleGroupAssociation",
                 "GetFirewallRuleGroupPolicy",
+                "GetOutpostResolver",
                 "GetResolverConfig",
                 "GetResolverDnssecConfig",
                 "GetResolverEndpoint",
                 "GetResolverQueryLogConfig",
                 "GetResolverQueryLogConfigAssociation",
                 "GetResolverQueryLogConfigPolicy",
                 "GetResolverRule",
@@ -18165,14 +18178,15 @@
                 "ImportFirewallDomains",
                 "ListFirewallConfigs",
                 "ListFirewallDomainLists",
                 "ListFirewallDomains",
                 "ListFirewallRuleGroupAssociations",
                 "ListFirewallRuleGroups",
                 "ListFirewallRules",
+                "ListOutpostResolvers",
                 "ListResolverConfigs",
                 "ListResolverDnssecConfigs",
                 "ListResolverEndpointIpAddresses",
                 "ListResolverEndpoints",
                 "ListResolverQueryLogConfigAssociations",
                 "ListResolverQueryLogConfigs",
                 "ListResolverRuleAssociations",
@@ -18183,14 +18197,15 @@
                 "PutResolverRulePolicy",
                 "TagResource",
                 "UntagResource",
                 "UpdateFirewallConfig",
                 "UpdateFirewallDomains",
                 "UpdateFirewallRule",
                 "UpdateFirewallRuleGroupAssociation",
+                "UpdateOutpostResolver",
                 "UpdateResolverConfig",
                 "UpdateResolverDnssecConfig",
                 "UpdateResolverEndpoint",
                 "UpdateResolverRule"
             ],
             "HasResource": true,
             "StringPrefix": "route53resolver",
```

### Comparing `iam_actions-1.2.20230725/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230726/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230725/iam_actions/services.json` & `iam_actions-1.2.20230726/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999617288832605%*

 * *Differences: {"'healthlake'": "{'ServiceNames': ['AWS HealthLake'], 'ARNFormats': "*

 * *                 "['arn:aws:healthlake:${Region}:${Account}:${ResourceType}/${ResourceName}']}",*

 * * "'omics'": "{'ServiceNames': ['AWS HealthOmics']}",*

 * * "'profile'": "{'Actions': {insert: [(25, 'GetSimilarProfiles'), (38, 'ListRuleBasedMatches')]}}",*

 * * "'quicksight'": "{'Actions': {insert: [(63, 'DescribeDashboardSnapshotJob'), (64, "*

 * *                 "'DescribeDashboardSnapshotJobResult'), (146, 'SearchUsers'), (150, "*

 * *                 "'S […]*

```diff
@@ -9868,15 +9868,15 @@
         "HasResource": true,
         "ServiceNames": [
             "AWS Health APIs and Notifications"
         ]
     },
     "healthlake": {
         "ARNFormats": [
-            "arn:aws:healthlake:${Region}:${AccountId}:${ResourceType}/${ResourceName}"
+            "arn:aws:healthlake:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:healthlake:.+:.+:.+"
         ],
         "Actions": [
             "CreateFHIRDatastore",
             "CreateResource",
@@ -9902,15 +9902,15 @@
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
-            "Amazon HealthLake"
+            "AWS HealthLake"
         ]
     },
     "honeycode": {
         "ARNFormats": [
             "arn:aws:honeycode:${Region}:${Account}:${ResourceType}:${ResourcePath}"
         ],
         "ARNRegexes": [
@@ -14815,15 +14815,15 @@
             "omics:AnnotationImportJobJobId",
             "omics:AnnotationStoreName",
             "omics:VariantImportJobJobId",
             "omics:VariantStoreName"
         ],
         "HasResource": true,
         "ServiceNames": [
-            "Amazon Omics"
+            "AWS HealthOmics"
         ]
     },
     "opsworks": {
         "ARNFormats": [
             "arn:aws:${ServiceName}:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
@@ -15484,26 +15484,28 @@
             "GetDomain",
             "GetEventStream",
             "GetIdentityResolutionJob",
             "GetIntegration",
             "GetMatches",
             "GetProfileObjectType",
             "GetProfileObjectTypeTemplate",
+            "GetSimilarProfiles",
             "GetWorkflow",
             "GetWorkflowSteps",
             "ListAccountIntegrations",
             "ListCalculatedAttributeDefinitions",
             "ListCalculatedAttributesForProfile",
             "ListDomains",
             "ListEventStreams",
             "ListIdentityResolutionJobs",
             "ListIntegrations",
             "ListProfileObjectTypeTemplates",
             "ListProfileObjectTypes",
             "ListProfileObjects",
+            "ListRuleBasedMatches",
             "ListTagsForResource",
             "ListWorkflows",
             "MergeProfiles",
             "PutIntegration",
             "PutProfileObject",
             "PutProfileObjectType",
             "SearchProfiles",
@@ -15807,14 +15809,16 @@
             "DescribeAnalysis",
             "DescribeAnalysisPermissions",
             "DescribeAssetBundleExportJob",
             "DescribeAssetBundleImportJob",
             "DescribeCustomPermissions",
             "DescribeDashboard",
             "DescribeDashboardPermissions",
+            "DescribeDashboardSnapshotJob",
+            "DescribeDashboardSnapshotJobResult",
             "DescribeDataSet",
             "DescribeDataSetPermissions",
             "DescribeDataSetRefreshProperties",
             "DescribeDataSource",
             "DescribeDataSourcePermissions",
             "DescribeEmailCustomizationTemplate",
             "DescribeFolder",
@@ -15888,17 +15892,19 @@
             "SearchAnalyses",
             "SearchDashboards",
             "SearchDataSets",
             "SearchDataSources",
             "SearchDirectoryGroups",
             "SearchFolders",
             "SearchGroups",
+            "SearchUsers",
             "SetGroupMapping",
             "StartAssetBundleExportJob",
             "StartAssetBundleImportJob",
+            "StartDashboardSnapshotJob",
             "Subscribe",
             "TagResource",
             "Unsubscribe",
             "UntagResource",
             "UpdateAccountCustomization",
             "UpdateAccountSettings",
             "UpdateAnalysis",
@@ -17235,32 +17241,35 @@
             "AssociateFirewallRuleGroup",
             "AssociateResolverEndpointIpAddress",
             "AssociateResolverQueryLogConfig",
             "AssociateResolverRule",
             "CreateFirewallDomainList",
             "CreateFirewallRule",
             "CreateFirewallRuleGroup",
+            "CreateOutpostResolver",
             "CreateResolverEndpoint",
             "CreateResolverQueryLogConfig",
             "CreateResolverRule",
             "DeleteFirewallDomainList",
             "DeleteFirewallRule",
             "DeleteFirewallRuleGroup",
+            "DeleteOutpostResolver",
             "DeleteResolverEndpoint",
             "DeleteResolverQueryLogConfig",
             "DeleteResolverRule",
             "DisassociateFirewallRuleGroup",
             "DisassociateResolverEndpointIpAddress",
             "DisassociateResolverQueryLogConfig",
             "DisassociateResolverRule",
             "GetFirewallConfig",
             "GetFirewallDomainList",
             "GetFirewallRuleGroup",
             "GetFirewallRuleGroupAssociation",
             "GetFirewallRuleGroupPolicy",
+            "GetOutpostResolver",
             "GetResolverConfig",
             "GetResolverDnssecConfig",
             "GetResolverEndpoint",
             "GetResolverQueryLogConfig",
             "GetResolverQueryLogConfigAssociation",
             "GetResolverQueryLogConfigPolicy",
             "GetResolverRule",
@@ -17269,14 +17278,15 @@
             "ImportFirewallDomains",
             "ListFirewallConfigs",
             "ListFirewallDomainLists",
             "ListFirewallDomains",
             "ListFirewallRuleGroupAssociations",
             "ListFirewallRuleGroups",
             "ListFirewallRules",
+            "ListOutpostResolvers",
             "ListResolverConfigs",
             "ListResolverDnssecConfigs",
             "ListResolverEndpointIpAddresses",
             "ListResolverEndpoints",
             "ListResolverQueryLogConfigAssociations",
             "ListResolverQueryLogConfigs",
             "ListResolverRuleAssociations",
@@ -17287,14 +17297,15 @@
             "PutResolverRulePolicy",
             "TagResource",
             "UntagResource",
             "UpdateFirewallConfig",
             "UpdateFirewallDomains",
             "UpdateFirewallRule",
             "UpdateFirewallRuleGroupAssociation",
+            "UpdateOutpostResolver",
             "UpdateResolverConfig",
             "UpdateResolverDnssecConfig",
             "UpdateResolverEndpoint",
             "UpdateResolverRule"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
@@ -19601,14 +19612,16 @@
             "ssm:AutoApprove",
             "ssm:DocumentCategories",
             "ssm:Overwrite",
             "ssm:Recursive",
             "ssm:SessionDocumentAccessCheck",
             "ssm:SyncType",
             "ssm:resourceTag/${TagKey}",
+            "ssm:resourceTag/aws:ssmmessages:session-id",
+            "ssm:resourceTag/aws:ssmmessages:target-id",
             "ssm:resourceTag/tag-key"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Systems Manager"
         ]
     },
@@ -19753,14 +19766,15 @@
             "ListComponents",
             "ListDatabases",
             "ListOperations",
             "ListTagsForResource",
             "PutResourcePermission",
             "RegisterApplication",
             "RestoreDatabase",
+            "StartApplicationRefresh",
             "TagResource",
             "UntagResource",
             "UpdateApplicationSettings",
             "UpdateHANABackupSettings"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
@@ -20744,14 +20758,15 @@
             "ListUsers",
             "ListWorkflows",
             "SendWorkflowStepState",
             "StartFileTransfer",
             "StartServer",
             "StopServer",
             "TagResource",
+            "TestConnection",
             "TestIdentityProvider",
             "UntagResource",
             "UpdateAccess",
             "UpdateAgreement",
             "UpdateCertificate",
             "UpdateConnector",
             "UpdateHostKey",
```

### Comparing `iam_actions-1.2.20230725/pyproject.toml` & `iam_actions-1.2.20230726/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230725"
+version = "1.2.20230726"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230725/setup.py` & `iam_actions-1.2.20230726/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230725',
+    'version': '1.2.20230726',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230725/PKG-INFO` & `iam_actions-1.2.20230726/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230725
+Version: 1.2.20230726
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

