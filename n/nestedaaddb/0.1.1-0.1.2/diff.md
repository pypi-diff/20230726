# Comparing `tmp/nestedaaddb-0.1.1.tar.gz` & `tmp/nestedaaddb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestedaaddb-0.1.1.tar", last modified: Mon Feb 20 11:31:46 2023, max compression
+gzip compressed data, was "nestedaaddb-0.1.2.tar", last modified: Wed Jul 26 01:28:36 2023, max compression
```

## Comparing `nestedaaddb-0.1.1.tar` & `nestedaaddb-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-02-20 11:31:46.607832 nestedaaddb-0.1.1/
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4797 2023-02-20 11:31:46.607599 nestedaaddb-0.1.1/PKG-INFO
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4371 2023-02-19 23:43:58.000000 nestedaaddb-0.1.1/README.md
-drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-02-20 11:31:46.605576 nestedaaddb-0.1.1/nestedaaddb/
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       79 2023-02-19 03:38:52.000000 nestedaaddb-0.1.1/nestedaaddb/__init__.py
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     6732 2022-11-15 23:54:32.000000 nestedaaddb-0.1.1/nestedaaddb/databricks_client.py
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4486 2022-11-16 07:00:43.000000 nestedaaddb-0.1.1/nestedaaddb/graph_client.py
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     5937 2023-02-19 05:00:39.000000 nestedaaddb-0.1.1/nestedaaddb/nested_groups.py
-drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-02-20 11:31:46.607280 nestedaaddb-0.1.1/nestedaaddb.egg-info/
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4797 2023-02-20 11:31:46.000000 nestedaaddb-0.1.1/nestedaaddb.egg-info/PKG-INFO
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)      321 2023-02-20 11:31:46.000000 nestedaaddb-0.1.1/nestedaaddb.egg-info/SOURCES.txt
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)        1 2023-02-20 11:31:46.000000 nestedaaddb-0.1.1/nestedaaddb.egg-info/dependency_links.txt
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       26 2023-02-20 11:31:46.000000 nestedaaddb-0.1.1/nestedaaddb.egg-info/requires.txt
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       12 2023-02-20 11:31:46.000000 nestedaaddb-0.1.1/nestedaaddb.egg-info/top_level.txt
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)      628 2023-02-20 11:31:10.000000 nestedaaddb-0.1.1/pyproject.toml
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       38 2023-02-20 11:31:46.607907 nestedaaddb-0.1.1/setup.cfg
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       38 2022-05-20 15:06:37.000000 nestedaaddb-0.1.1/setup.py
+drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-07-26 01:28:36.248365 nestedaaddb-0.1.2/
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     5196 2023-07-26 01:28:36.248209 nestedaaddb-0.1.2/PKG-INFO
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4770 2023-07-26 00:42:05.000000 nestedaaddb-0.1.2/README.md
+drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-07-26 01:28:36.246490 nestedaaddb-0.1.2/nestedaaddb/
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       79 2023-02-19 03:38:52.000000 nestedaaddb-0.1.2/nestedaaddb/__init__.py
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     6928 2023-03-07 06:13:17.000000 nestedaaddb-0.1.2/nestedaaddb/databricks_client.py
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4486 2022-11-16 07:00:43.000000 nestedaaddb-0.1.2/nestedaaddb/graph_client.py
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4432 2023-03-07 05:27:06.000000 nestedaaddb-0.1.2/nestedaaddb/nested_groups.py
+drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-07-26 01:28:36.247957 nestedaaddb-0.1.2/nestedaaddb.egg-info/
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     5196 2023-07-26 01:28:36.000000 nestedaaddb-0.1.2/nestedaaddb.egg-info/PKG-INFO
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)      321 2023-07-26 01:28:36.000000 nestedaaddb-0.1.2/nestedaaddb.egg-info/SOURCES.txt
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)        1 2023-07-26 01:28:36.000000 nestedaaddb-0.1.2/nestedaaddb.egg-info/dependency_links.txt
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       39 2023-07-26 01:28:36.000000 nestedaaddb-0.1.2/nestedaaddb.egg-info/requires.txt
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       12 2023-07-26 01:28:36.000000 nestedaaddb-0.1.2/nestedaaddb.egg-info/top_level.txt
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)      643 2023-07-26 01:19:53.000000 nestedaaddb-0.1.2/pyproject.toml
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       38 2023-07-26 01:28:36.248415 nestedaaddb-0.1.2/setup.cfg
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       38 2022-05-20 15:06:37.000000 nestedaaddb-0.1.2/setup.py
```

### Comparing `nestedaaddb-0.1.1/PKG-INFO` & `nestedaaddb-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaaddb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package that allows to sync Nested AAD Group to DataBricks
 Author-email: Abhishek Pratap Singh <sumoaps@outlook.com>
 Keywords: Databricks,SCIM,nested AAD
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -79,15 +79,24 @@
   
   * In the Application permissions section, ensure that the **right permissions are checked: User.Read.All**
   
   * Select the Add permissions button at the bottom.
   
 10.At this stage, the permissions are assigned correctly but since the client app does not allow users to interact, the user's themselves cannot consent to these permissions. To get around this problem, we'd let the tenant administrator consent on behalf of all users in the tenant. Click the Grant admin consent for {tenant} button, and then select Yes when you are asked if you want to grant consent for the requested permissions for all account in the tenant. You need to be the tenant admin to be able to carry out this operation.
 
-##  Step (ii) 
+
+##  Step (i) 
+**Populate config.cfg files with Databricks Settings**
+Extract the SCIM Token and ACCOUNT SCIM URL Details: https://learn.microsoft.com/en-us/azure/databricks/administration-guide/users-groups/scim/aad#step-1-configure-azure-databricks
+
+![Screenshot 2023-04-24 at 8 17 17 pm](https://user-images.githubusercontent.com/110456615/233968828-ac9ecee3-e996-45c5-8854-e31dfadd5d87.png)
+
+
+
+##  Step (iii) 
 ## Running the app
 
 ### As Standalon Python app:
 * Install utility via pip
 
 ````
 pip install nestedaaddb
```

### Comparing `nestedaaddb-0.1.1/README.md` & `nestedaaddb-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,24 @@
   
   * In the Application permissions section, ensure that the **right permissions are checked: User.Read.All**
   
   * Select the Add permissions button at the bottom.
   
 10.At this stage, the permissions are assigned correctly but since the client app does not allow users to interact, the user's themselves cannot consent to these permissions. To get around this problem, we'd let the tenant administrator consent on behalf of all users in the tenant. Click the Grant admin consent for {tenant} button, and then select Yes when you are asked if you want to grant consent for the requested permissions for all account in the tenant. You need to be the tenant admin to be able to carry out this operation.
 
-##  Step (ii) 
+
+##  Step (i) 
+**Populate config.cfg files with Databricks Settings**
+Extract the SCIM Token and ACCOUNT SCIM URL Details: https://learn.microsoft.com/en-us/azure/databricks/administration-guide/users-groups/scim/aad#step-1-configure-azure-databricks
+
+![Screenshot 2023-04-24 at 8 17 17 pm](https://user-images.githubusercontent.com/110456615/233968828-ac9ecee3-e996-45c5-8854-e31dfadd5d87.png)
+
+
+
+##  Step (iii) 
 ## Running the app
 
 ### As Standalon Python app:
 * Install utility via pip
 
 ````
 pip install nestedaaddb
```

### Comparing `nestedaaddb-0.1.1/nestedaaddb/databricks_client.py` & `nestedaaddb-0.1.2/nestedaaddb/databricks_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,27 +73,29 @@
                 if "members" in dbg:
                     for dbmember in dbg["members"]:
                         '''
                         If it is user we are storing both name and email
                         If group we only store name
                         check if user or group exists
                         '''
-                        if (member["type"] == "user" and member["data"][0].casefold() == dbmember["display"].casefold())\
-                                or (member["type"] == "group" and member["data"].casefold() == dbmember["display"].casefold()):
+                        if (member["type"] == "user" and member["data"][0].casefold() == dbmember["display"].casefold()) \
+                                or (member["type"] == "group" and member["data"].casefold() == dbmember[
+                            "display"].casefold()):
                             exists = True
                             break
                 if not exists:
                     toadd.append(member)
 
         if "members" in dbg:
             for dbmember in dbg["members"]:
                 exists = False
                 for member in members:
                     if (member["type"] == "user" and member["data"][0].casefold() == dbmember["display"].casefold()) \
-                            or (member["type"] == "group" and member["data"].casefold() == dbmember["display"].casefold()):
+                            or (
+                            member["type"] == "group" and member["data"].casefold() == dbmember["display"].casefold()):
                         exists = True
                         break
                 if not exists:
                     toremove.append(dbmember)
 
         ops = []
 
@@ -110,28 +112,29 @@
                         if dbu["displayName"].casefold() == member["data"][0].casefold() and dbu["userName"].casefold() == member["data"][1].casefold():
                             obj = dict()
                             obj["value"] = dbu["id"]
                             mem.append(obj)
                             break
                 # or if it is a group
                 elif member["type"] == "group":
-                    for dbg in dbgroups["Resources"]:
-                        if dbg["displayName"].casefold() == member["data"].casefold():
+                    for dbgg in dbgroups["Resources"]:
+                        if dbgg["displayName"].casefold() == member["data"].casefold():
                             obj = dict()
-                            obj["value"] = dbg["id"]
+                            obj["value"] = dbgg["id"]
                             mem.append(obj)
                             break
 
             dictmem = {"members": mem}
             dictsub = {'op': "add", 'path': "members", 'value': dictmem}
             ops.append(dictsub)
 
         if len(toremove) > 0:
             mem = []
             for member in toremove:
+                obj = dict()
                 obj["value"] = member["value"]
                 mem.append(obj)
 
             dictmem = {"members": mem}
             dictsub = {'op': "remove", 'path': "members", 'value': dictmem}
             ops.append(dictsub)
 
@@ -141,15 +144,17 @@
         my_headers = {'Authorization': 'Bearer ' + self.dbscimToken}
         if not dryrun:
             response = requests.patch(api_url, data=ujson, headers=my_headers)
             print("Group Existed but membership updated. Request was :" + ujson)
             print("Response was :" + response.text)
 
         else:
-            print("Group Exists but membership need to be updated for :" + dbg["displayName"])
+            print("Group Exists but membership need to be updated for :"
+                  + dbg[
+                      "displayName"] + ". Request details-> data " + ujson + ",EndPoint :" + api_url)
 
     '''
     Get all Databricks groups
     '''
 
     def get_dbgroups(self):
         api_url = self.dbbaseUrl + "/Groups"
```

### Comparing `nestedaaddb-0.1.1/nestedaaddb/graph_client.py` & `nestedaaddb-0.1.2/nestedaaddb/graph_client.py`

 * *Files identical despite different names*

### Comparing `nestedaaddb-0.1.1/nestedaaddb/nested_groups.py` & `nestedaaddb-0.1.2/nestedaaddb/nested_groups.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,17 +26,16 @@
         azure_settings = self.config['azure']
         db_settings = self.config['databricks']
 
         self.graph: Graph = Graph(azure_settings)
         self.dbclient: DatabricksClient = DatabricksClient(db_settings)
 
     '''
-    
+    Peforms sync of Users and Groups
     '''
-
     def sync(self, toplevelgroup, dryrun=False):
 
         '''
         Read All Databricks users and groups
         '''
         dbusers = self.dbclient.get_dbusers()
         dbgroups = self.dbclient.get_dbgroups()
@@ -48,96 +47,78 @@
         '''
         groups_page = self.graph.get_groups()
 
         print("2.All AAD groups Read done")
 
         print("3.Top level group requested is " + toplevelgroup)
 
+
         '''
         Indicates whether user and group collection are loaded successfully
         '''
-        for top in toplevelgroup.split(","):
+        colInitialised = False
+
+        '''
+        Iterate through each group in AAD and map members corresponding to it including nested child group members
+        '''
+        for group in groups_page['value']:
+            print("Group is " + group["displayName"])
+
+            if toplevelgroup != "" and toplevelgroup.casefold() == group["displayName"].casefold():
+                distinct_groupsU, distinct_usersU, groupgpU = self.graph.extract_children_from_group(self.graph,
+                                                                                                     group["id"],
+                                                                                                     group[
+                                                                                                         "displayName"],
+                                                                                                     self.distinct_groups,
+                                                                                                     self.distinct_users,
+                                                                                                     self.groupgp);
+                colInitialised = True
+
+        print("4.Hierarchy analysed,going to create users and groups")
+
+        if dryrun:
+            print("THIS IS DRY RUN.NO CHANGES WILL TAKE PLACE ON DATABRICKS")
+
+        if colInitialised:
+
+            '''
+            Create Users and groups in Databricks as required
+            '''
+            for u in distinct_usersU:
 
-            self.distinct_groups.clear()
-            self.distinct_users.clear()
-            self.groupgp.clear()
-
-            colInitialised = False
-
-            '''
-            Iterate through each group in AAD and map members corresponding to it including nested child group members
-            '''
-            for group in groups_page['value']:
-                print("Group is " + group["displayName"])
-
-                '''
-                If this is invoked via cli with program arguments
-                '''
-                if len(sys.argv[1:]) > 0:
-                    for arg in sys.argv[1:]:
-                        if not arg.startswith("--") and top.casefold() == group["displayName"].casefold():
-                            distinct_groupsU, distinct_usersU, groupgpU = self.graph.extract_children_from_group(self.graph,
-                                                                                                            group["id"],
-                                                                                                            group[
-                                                                                                                "displayName"],
-                                                                                                            self.distinct_groups,
-                                                                                                            self.distinct_users,
-                                                                                                            self.groupgp);
-                            colInitialised = True
-                elif top != "" and top.casefold() == group["displayName"].casefold():
-                    distinct_groupsU, distinct_usersU, groupgpU = self.graph.extract_children_from_group(self.graph,
-                                                                                                    group["id"],
-                                                                                                    group[
-                                                                                                        "displayName"],
-                                                                                                    self.distinct_groups,
-                                                                                                    self.distinct_users,
-                                                                                                    self.groupgp);
-                    colInitialised = True
-
-            print("4.Hierarchy analysed,going to create users and groups")
-
-            if dryrun:
-                print("THIS IS DRY RUN.NO CHANGES WILL TAKE PLACE ON DATABRICKS")
-
-            if colInitialised:
-
-                '''
-                Create Users and groups in Databricks as required
-                '''
-                for u in distinct_usersU:
-
-                    exists = False
-
-                    for udb in dbusers["Resources"]:
-                        if u[0].casefold() == udb["displayName"].casefold():
-                            exists = True;
-
-                    if not exists:
-                        self.dbclient.create_dbuser(u, dryrun)
-
-                for u in distinct_groupsU:
-                    exists = False
-                    for dbg in dbgroups["Resources"]:
-                        if u.casefold() == dbg["displayName"].casefold():
-                            exists = True
-
-                    if not exists:
-                        self.dbclient.create_blank_dbgroup(u, dryrun)
-
-                '''
-                Reloading users from Databricks as we need id of new users as well added in last step
-                '''
-                dbusers = self.dbclient.get_dbusers()
-                dbgroups = self.dbclient.get_dbgroups()
-
-                '''
-                Create groups or update membership of groups i.e. add/remove users from groups
-                '''
-                for u in distinct_groupsU:
-                    exists = False
-                    for dbg in dbgroups["Resources"]:
-                        if u.casefold() == dbg["displayName"].casefold():
-                            exists = True
-                            # compare and add remove the members as needed
-                            self.dbclient.patch_dbgroup(dbg["id"], groupgpU.get(u), dbg, dbusers, dbgroups, dryrun)
+                exists = False
 
+                for udb in dbusers["Resources"]:
+                    if u[0].casefold() == udb["displayName"].casefold():
+                        exists = True;
+
+                if not exists:
+                    self.dbclient.create_dbuser(u, dryrun)
+
+            for u in distinct_groupsU:
+                exists = False
+                for dbg in dbgroups["Resources"]:
+                    if u.casefold() == dbg["displayName"].casefold():
+                        exists = True
+
+                if not exists:
+                    self.dbclient.create_blank_dbgroup(u, dryrun)
+
+            '''
+            Reloading users from Databricks as we need id of new users as well added in last step
+            '''
+            dbusers = self.dbclient.get_dbusers()
+            dbgroups = self.dbclient.get_dbgroups()
+
+            '''
+            Create groups or update membership of groups i.e. add/remove users from groups
+            '''
+            for u in distinct_groupsU:
+                exists = False
+                for dbg in dbgroups["Resources"]:
+                    if u.casefold() == dbg["displayName"].casefold():
+                        exists = True
+                        # compare and add remove the members as needed
+                        self.dbclient.patch_dbgroup(dbg["id"], groupgpU.get(u), dbg, dbusers, dbgroups, dryrun)
         print("All Operation completed !")
+
+
```

### Comparing `nestedaaddb-0.1.1/nestedaaddb.egg-info/PKG-INFO` & `nestedaaddb-0.1.2/nestedaaddb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestedaaddb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package that allows to sync Nested AAD Group to DataBricks
 Author-email: Abhishek Pratap Singh <sumoaps@outlook.com>
 Keywords: Databricks,SCIM,nested AAD
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -79,15 +79,24 @@
   
   * In the Application permissions section, ensure that the **right permissions are checked: User.Read.All**
   
   * Select the Add permissions button at the bottom.
   
 10.At this stage, the permissions are assigned correctly but since the client app does not allow users to interact, the user's themselves cannot consent to these permissions. To get around this problem, we'd let the tenant administrator consent on behalf of all users in the tenant. Click the Grant admin consent for {tenant} button, and then select Yes when you are asked if you want to grant consent for the requested permissions for all account in the tenant. You need to be the tenant admin to be able to carry out this operation.
 
-##  Step (ii) 
+
+##  Step (i) 
+**Populate config.cfg files with Databricks Settings**
+Extract the SCIM Token and ACCOUNT SCIM URL Details: https://learn.microsoft.com/en-us/azure/databricks/administration-guide/users-groups/scim/aad#step-1-configure-azure-databricks
+
+![Screenshot 2023-04-24 at 8 17 17 pm](https://user-images.githubusercontent.com/110456615/233968828-ac9ecee3-e996-45c5-8854-e31dfadd5d87.png)
+
+
+
+##  Step (iii) 
 ## Running the app
 
 ### As Standalon Python app:
 * Install utility via pip
 
 ````
 pip install nestedaaddb
```

### Comparing `nestedaaddb-0.1.1/pyproject.toml` & `nestedaaddb-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nestedaaddb"
-version = "0.1.1"
+version = "0.1.2"
 description = "A package that allows to sync Nested AAD Group to DataBricks"
 readme = "README.md"
 authors = [{ name = "Abhishek Pratap Singh", email = "sumoaps@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ['Databricks', 'SCIM', 'nested AAD']
-dependencies = ['azure-core', 'azure-identity']
+dependencies = ['azure-core', 'azure-identity','msgraph-core']
 requires-python = ">=3.7"
```

