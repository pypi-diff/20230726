# Comparing `tmp/cfntagger-0.9.7-py3-none-any.whl.zip` & `tmp/cfntagger-0.9.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 25038 bytes, number of entries: 19
--rw-r--r--  2.0 unx       30 b- defN 22-Apr-28 14:49 cfntagger/__init__.py
--rw-r--r--  2.0 unx    16549 b- defN 22-Jul-14 10:13 cfntagger/cfntagger.py
--rwxr-xr-x  2.0 unx     1671 b- defN 22-Jul-15 04:39 cfntagger-0.9.7.data/scripts/cfntagger
--rw-r--r--  2.0 unx        0 b- defN 22-Apr-28 11:31 tests/__init__.py
--rw-r--r--  2.0 unx     2462 b- defN 22-May-02 06:37 tests/test_canary.py
--rw-r--r--  2.0 unx     1087 b- defN 22-Jun-20 07:04 tests/test_comments.py
--rw-r--r--  2.0 unx     2153 b- defN 22-May-02 06:37 tests/test_ec2.py
--rw-r--r--  2.0 unx      829 b- defN 22-Jul-14 10:13 tests/test_empty_cfntags.py
--rw-r--r--  2.0 unx     1247 b- defN 22-Jun-20 07:04 tests/test_get_kv.py
--rw-r--r--  2.0 unx      793 b- defN 22-May-31 07:22 tests/test_noproperties.py
--rw-r--r--  2.0 unx     2422 b- defN 22-May-03 09:19 tests/test_s3.py
--rw-r--r--  2.0 unx     1734 b- defN 22-Jun-20 07:04 tests/test_s3_output_is_cfn.py
--rw-r--r--  2.0 unx     1488 b- defN 22-Jun-20 07:04 tests/test_supports_tags.py
--rw-r--r--  2.0 unx     1442 b- defN 22-Jun-20 07:04 tests/unittest.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Jul-15 04:39 cfntagger-0.9.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      611 b- defN 22-Jul-15 04:39 cfntagger-0.9.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-15 04:39 cfntagger-0.9.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 22-Jul-15 04:39 cfntagger-0.9.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1508 b- defN 22-Jul-15 04:39 cfntagger-0.9.7.dist-info/RECORD
-19 files, 71283 bytes uncompressed, 22594 bytes compressed:  68.3%
+Zip file size: 25953 bytes, number of entries: 20
+-rw-r--r--  2.0 unx       30 b- defN 22-Jun-25 14:17 cfntagger/__init__.py
+-rw-r--r--  2.0 unx    17897 b- defN 22-Jul-21 21:16 cfntagger/cfntagger.py
+-rwxr-xr-x  2.0 unx     1671 b- defN 22-Jul-22 14:30 cfntagger-0.9.8.data/scripts/cfntagger
+-rw-r--r--  2.0 unx        0 b- defN 22-Jun-25 14:17 tests/__init__.py
+-rw-r--r--  2.0 unx     2462 b- defN 22-Jun-25 14:17 tests/test_canary.py
+-rw-r--r--  2.0 unx     1087 b- defN 22-Jun-25 14:17 tests/test_comments.py
+-rw-r--r--  2.0 unx     2153 b- defN 22-Jun-25 14:17 tests/test_ec2.py
+-rw-r--r--  2.0 unx      829 b- defN 22-Jul-14 18:26 tests/test_empty_cfntags.py
+-rw-r--r--  2.0 unx     1247 b- defN 22-Jun-25 14:17 tests/test_get_kv.py
+-rw-r--r--  2.0 unx      849 b- defN 22-Jul-21 21:16 tests/test_git.py
+-rw-r--r--  2.0 unx      793 b- defN 22-Jun-25 14:17 tests/test_noproperties.py
+-rw-r--r--  2.0 unx     2422 b- defN 22-Jun-25 14:17 tests/test_s3.py
+-rw-r--r--  2.0 unx     1734 b- defN 22-Jun-25 14:17 tests/test_s3_output_is_cfn.py
+-rw-r--r--  2.0 unx     1488 b- defN 22-Jun-25 14:17 tests/test_supports_tags.py
+-rw-r--r--  2.0 unx     1442 b- defN 22-Jun-25 14:17 tests/unittest.py
+-rw-r--r--  2.0 unx    35149 b- defN 22-Jul-22 14:30 cfntagger-0.9.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      611 b- defN 22-Jul-22 14:30 cfntagger-0.9.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Jul-22 14:30 cfntagger-0.9.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 22-Jul-22 14:30 cfntagger-0.9.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1581 b- defN 22-Jul-22 14:30 cfntagger-0.9.8.dist-info/RECORD
+20 files, 73553 bytes uncompressed, 23399 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
 Filename: cfntagger/__init__.py
 Comment: 
 
 Filename: cfntagger/cfntagger.py
 Comment: 
 
-Filename: cfntagger-0.9.7.data/scripts/cfntagger
+Filename: cfntagger-0.9.8.data/scripts/cfntagger
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_canary.py
 Comment: 
@@ -21,14 +21,17 @@
 
 Filename: tests/test_empty_cfntags.py
 Comment: 
 
 Filename: tests/test_get_kv.py
 Comment: 
 
+Filename: tests/test_git.py
+Comment: 
+
 Filename: tests/test_noproperties.py
 Comment: 
 
 Filename: tests/test_s3.py
 Comment: 
 
 Filename: tests/test_s3_output_is_cfn.py
@@ -36,23 +39,23 @@
 
 Filename: tests/test_supports_tags.py
 Comment: 
 
 Filename: tests/unittest.py
 Comment: 
 
-Filename: cfntagger-0.9.7.dist-info/LICENSE
+Filename: cfntagger-0.9.8.dist-info/LICENSE
 Comment: 
 
-Filename: cfntagger-0.9.7.dist-info/METADATA
+Filename: cfntagger-0.9.8.dist-info/METADATA
 Comment: 
 
-Filename: cfntagger-0.9.7.dist-info/WHEEL
+Filename: cfntagger-0.9.8.dist-info/WHEEL
 Comment: 
 
-Filename: cfntagger-0.9.7.dist-info/top_level.txt
+Filename: cfntagger-0.9.8.dist-info/top_level.txt
 Comment: 
 
-Filename: cfntagger-0.9.7.dist-info/RECORD
+Filename: cfntagger-0.9.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cfntagger/cfntagger.py

```diff
@@ -1,9 +1,10 @@
 from collections import OrderedDict
 import os
+import re
 import sys
 import json
 from typing import List, Dict
 import git
 from ruamel.yaml import YAML
 from colorama import Fore, Style
 
@@ -270,37 +271,85 @@
             sys.exit(1)
         else:
             self.resources = self.data.get("Resources")
             self.obligatory_tags = obligatory_tags
 
 
     def get_updated_tags(self, resource: str) -> List:
+        """
+        Returns a list of the changed tags for a resource
+        """
         try:
             return self.stats[resource]["updatedtags"]
         except KeyError:
             return []
 
 
     def get_obligatory_tags(self) -> Dict:
         return self.obligatory_tags
 
 
     def get_found_tags(self, resource: str) -> List:
+        """
+        Returns a list of the present tags on a resource
+        """
         try:
             return self.stats[resource]["foundtags"]
         except KeyError:
             return []
 
 
     def get_added_tags(self, resource: str) -> List:
+        """
+        Returns a list of the added tags for a resource
+        """
+
         try:
             return self.stats[resource]["addedtags"]
         except KeyError:
             return []
 
+    def get_git_path(self, filename: str) -> str:
+        """
+        Returns the relative path for a file from the repo root dir
+        instead of any abritrary path the user has given us
+        """
+
+        if filename.startswith('./'):
+            filename = filename.replace('./', '')
+
+        full_path = os.getcwd()
+        full_path_with_file = f"{full_path}/{filename}"
+        repo = git.Repo('.', search_parent_directories=True)
+        repodir = f"{repo.working_tree_dir}/"
+        relative_file_path = f"{full_path_with_file}".replace(repodir, '')
+
+        return relative_file_path
+
+
+    def get_git_tags(self, filename: str) -> dict:
+        """
+        Returns a dict of gitrepo & gitfile tags
+        """
+
+        if self.git:
+            try:
+                repo = git.Repo(os.getcwd(), search_parent_directories=True)
+                remote = repo.remote().url
+
+                # remove any tokens from the remote string
+                remote = re.sub('https://[a-zA-Z0-9_]+@', 'https://', remote)
+            except git.exc.InValidGitRepositoryError:
+                print("FAIL: this is no git repo, please drop the --git argument")
+                sys.exit(1)
+            else:
+                gitdict = { 'gitrepo': remote, 'gitfile': self.get_git_path(filename) }
+
+        return gitdict
+
 
     def change_tags(
         self, taglist: List[OrderedDict], resource: str
     ) -> List[OrderedDict]:
 
         resultlist = []
 
@@ -328,21 +377,14 @@
             else:
                 resultlist.append(OrderedDict({"Key": key, "Value": value}))
 
         return resultlist
 
 
     def tag(self):
-        if self.git:
-            try:
-                repo = git.Repo(os.getcwd(), search_parent_directories=True)
-                remote = repo.remote().url
-            except git.exc.InValidGitRepositoryError:
-                print("FAIL: this is no git repo, please drop the --git argument")
-                sys.exit(1)
 
         for item in self.resources:
             restype = self.resources[item].get("Type")
             if restype in self.resourcetypes_to_tag:
                 self.stats[item] = {"foundtags": [], "updatedtags": [], "addedtags": []}
                 print(" ")
                 print(
@@ -384,31 +426,32 @@
                             # So we need to add a Properties block.  Beware that we're in a
                             # obligtag loop, so only add it once
                             if not self.has_properties:
                                 self.resources[item].update({'Properties': OrderedDict({'Tags': [addtags]})})
                                 self.has_properties = True
 
                 if self.git:
+                    found_git_tags = self.get_git_tags(self.filename)
                     gittags = OrderedDict(
                         {
                             "Key": "gitrepo",
-                            "Value": remote
+                            "Value": found_git_tags['gitrepo']
                         }
                     )
                     if "Tags" in self.resources[item].get("Properties"):
                         self.resources[item].get("Properties").get("Tags").append(
                                 gittags
                         )
                     else:
                         self.resources[item]["Properties"]["Tags"] = [gittags]
 
                     gittags = OrderedDict(
                         {
                             "Key": "gitfile",
-                            "Value": self.filename
+                            "Value": found_git_tags['gitfile']
                         }
                     )
                     self.resources[item].get("Properties").get("Tags").append(
                             gittags
                     )
 
         yaml = YAML()
```

## Comparing `cfntagger-0.9.7.data/scripts/cfntagger` & `cfntagger-0.9.8.data/scripts/cfntagger`

 * *Files identical despite different names*

## Comparing `cfntagger-0.9.7.dist-info/LICENSE` & `cfntagger-0.9.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cfntagger-0.9.7.dist-info/METADATA` & `cfntagger-0.9.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfntagger
-Version: 0.9.7
+Version: 0.9.8
 Summary: A Cloudformation tagging tool
 Home-page: https://github.com/kristofwillen/cfntagger
 Author: Kristof Willen
 Author-email: kristof.willen@gmail.com
 License: GPL
 Keywords: cloudformation tagging
 Classifier: Programming Language :: Python :: 3
```

