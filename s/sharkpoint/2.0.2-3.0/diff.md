# Comparing `tmp/sharkpoint-2.0.2.tar.gz` & `tmp/sharkpoint-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharkpoint-2.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sharkpoint-3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sharkpoint-2.0.2.tar` & `sharkpoint-3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1059 2023-07-12 18:50:32.609034 sharkpoint-2.0.2/LICENSE
--rw-r--r--   0        0        0      508 2023-07-12 19:39:50.014951 sharkpoint-2.0.2/README.md
--rw-r--r--   0        0        0      966 2023-07-17 13:31:14.389925 sharkpoint-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      502 2023-07-17 12:24:18.004073 sharkpoint-2.0.2/src/sharkpoint/__init__.py
--rw-r--r--   0        0        0     2832 2023-07-14 15:01:59.312373 sharkpoint-2.0.2/src/sharkpoint/sharepoint.py
--rw-r--r--   0        0        0     9395 2023-07-17 13:28:19.415931 sharkpoint-2.0.2/src/sharkpoint/sharepoint_file.py
--rw-r--r--   0        0        0     8611 2023-07-17 12:24:18.005070 sharkpoint-2.0.2/src/sharkpoint/sharepoint_site.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 sharkpoint-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-12 18:50:32.609034 sharkpoint-3.0/LICENSE
+-rw-r--r--   0        0        0      508 2023-07-12 19:39:50.014951 sharkpoint-3.0/README.md
+-rw-r--r--   0        0        0     1002 2023-07-25 20:46:35.786246 sharkpoint-3.0/pyproject.toml
+-rw-r--r--   0        0        0      502 2023-07-17 12:24:18.004073 sharkpoint-3.0/src/sharkpoint/__init__.py
+-rw-r--r--   0        0        0     4276 2023-07-26 12:43:28.093500 sharkpoint-3.0/src/sharkpoint/sharepoint.py
+-rw-r--r--   0        0        0     9283 2023-07-26 12:48:45.449495 sharkpoint-3.0/src/sharkpoint/sharepoint_file.py
+-rw-r--r--   0        0        0    12825 2023-07-26 12:47:05.940729 sharkpoint-3.0/src/sharkpoint/sharepoint_site.py
+-rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 sharkpoint-3.0/PKG-INFO
```

### Comparing `sharkpoint-2.0.2/LICENSE` & `sharkpoint-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sharkpoint-2.0.2/pyproject.toml` & `sharkpoint-3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "sharkpoint"
-version = "2.0.2"
+version = "3.0"
 description = "A small Pythonic library for interacting with SharePoint document libraries"
 authors = [
   { name = "TheOtherOne" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
@@ -33,8 +33,11 @@
 addopts = "-ra -q"
 testpaths = [
     "tests",
 ]
 pythonpath = [
   "src"
 ]
-env_files = ".env_tests"
+env_files = ".env_tests"
+markers = [
+    "incremental",
+]
```

### Comparing `sharkpoint-2.0.2/src/sharkpoint/sharepoint.py` & `sharkpoint-3.0/src/sharkpoint/sharepoint.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import azure.identity
 import requests
 import json
 from . import sharepoint_site
-import azure.core.credentials
+from azure.core.credentials import TokenCredential
 
 
 class SharePoint:
     """
     A class used to represent an organization's SharePoint instance using the SharePoint REST API v1.
     ...
 
@@ -15,79 +14,113 @@
     base_url : str
         The URL of a Sharepoint instance, ex. contoso.sharepoint.com
     azure_identity : TokenCredential
         An azure-identity token credential.
 
     Attributes
     ----------
+    site_names : str
+        a list of all user-facing site names in SharePoint
     sites : dict
         a dictionary of all sites in SharePoint, the key is the user-facing name and the value is the URL
     base_url : str
         the URL of the SharePoint instance
 
     Methods
     -------
-    get_site(site_name)
+    get_site(site_name) : SharepointSite
         Returns a SharepointSite object for a specific SharePoint site
+    create_site(site_name, path, owner, description, web_template, lcid, site_design_id) : SharepointSite
+        Creates a new site and returns a SharepointSite object for the site
     """
 
     def __init__(
         self,
         sharepoint_url: str,
-        azure_identity: azure.core.credentials.TokenCredential,
+        azure_identity: TokenCredential,
     ) -> None:
         self.base_url = sharepoint_url
         self._scope = f"{self.base_url}/.default"
         self._identity = azure_identity
-        self.sites = self._initalize_sites()
 
     @property
     def _token(self):
         return self._identity.get_token(self._scope)
 
     @property
     def _header(self):
         return {
             "Authorization": f"Bearer {self._token.token}",
             "Accept": "application/json;odata=verbose",
             "Content-Type": "application/json;odata=verbose",
         }
 
-    def _initalize_sites(self):
-        api_url = f"{self.base_url}/_api/search/query?querytext='contentclass:STS_Site contentclass:STS_Web'&selectproperties='Title,Path'"
+    @property
+    def sites(self) -> dict:
+        api_url = f"{self.base_url}_api/search/query?querytext='contentclass:STS_Site'"
         request = requests.get(api_url, headers=self._header).text
         request = json.loads(request)
         # fmt: off
         request = request["d"]["query"]["PrimaryQueryResult"]["RelevantResults"]["Table"]["Rows"]["results"]
         # fmt: on
+        # By G-d Almighty this looks ugly, but this is the easiest way to parse the table for what I need
+        sites_dict = {
+            site["Cells"]["results"][2]["Value"]: site["Cells"]["results"][5]["Value"]
+            for site in request
+        }
+        return sites_dict
 
-        sites = []
-        for x in request:
-            site_dict = {
-                "Site Name": x["Cells"]["results"][0]["Value"],
-                "Site Path": x["Cells"]["results"][1]["Value"],
-            }
-            sites.append(site_dict)
-        return sites
-
-    def get_site(self, site_name):
+    def get_site(self, site_name: str) -> sharepoint_site.SharepointSite:
         """
         Parameters
         ----------
         site_name : str
             The user-facing name of a SharePoint site
 
         Raises
         ------
         KeyError
             If the subsite does not exist
 
         """
+        site_url = None
+        sites = self.sites
+        if site_name in sites.keys():
+            site_url = sites[site_name]
+        else:
+            raise KeyError("Site not found.")
 
-        site_url = next(
-            (item for item in self.sites if item["Site Name"] == site_name), None
+        return sharepoint_site.SharepointSite(site_url, self.base_url, self._header)
+
+    def create_site(
+        self,
+        site_name: str,
+        path: str,
+        owner: str,
+        description: str,
+        web_template: str = "sts#3",
+        lcid: int = 1033,
+        site_design_id: str = "00000000-0000-0000-0000-000000000000",
+    ) -> sharepoint_site.SharepointSite:
+        api_url = f"{self.base_url}/_api/SPSiteManager/create"
+        request = {
+            "request": {
+                "Title": site_name,
+                "Url": f"{self.base_url}/sites/{path}",
+                "Lcid": str(lcid),
+                "ShareByEmailEnabled": "false",
+                "Description": description,
+                "WebTemplate": web_template,
+                "SiteDesignId": site_design_id,
+                "Owner": owner,
+            }
+        }
+        request_return = requests.post(
+            api_url, data=json.dumps(request), headers=self._header
         )
-        if site_url is None:
-            raise KeyError("Site not found.")
+        request_return = json.loads(request_return.content)
+        if request_return["d"]["Create"]["SiteStatus"] == 2:
+            return sharepoint_site.SharepointSite(
+                request_return["d"]["Create"]["SiteUrl"], self.base_url, self._header
+            )
         else:
-            site_url = site_url["Site Path"]
-        return sharepoint_site.SharepointSite(site_url, self.base_url, self._header)
+            raise Exception(request_return["d"]["Create"]["SiteStatus"])
```

### Comparing `sharkpoint-2.0.2/src/sharkpoint/sharepoint_file.py` & `sharkpoint-3.0/src/sharkpoint/sharepoint_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,98 +48,97 @@
         if self._checkout:
             api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/CheckOut()"
             requests.post(api_url, headers=self._header)
 
         api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/$value"
         file = requests.get(api_url, headers=self._header)
         return file.content
-    
+
     def read(self, size: int = -1) -> bytes:
         if not self.readable():
             raise IOError("File not open in read mode.")
         return super().read(size)
-    
+
     def write(self, bytes):
         if not self.writable():
             raise IOError("File not open in write mode.")
         return super().write(bytes)
-    
+
     def truncate(self, __size: int | None = ...) -> int:
-            if not self.seekable():
-                raise IOError("File not open in seekable mode.")
-            return super().truncate(__size)
-    
+        if not self.seekable():
+            raise IOError("File not open in seekable mode.")
+        return super().truncate(__size)
+
     def readline(self, size: int = -1) -> str:
         if not self.readable():
             raise IOError("File not open in read mode.")
         return super().readline(size)
-    
+
     def readlines(self, size: int = -1) -> list[str]:
         if not self.readable():
             raise IOError("File not open in read mode.")
         return super().readlines(size)
-    
+
     def seek(self, cookie: int, whence: int = 0) -> int:
         if not self.seekable():
             raise IOError("File not open in seekable mode.")
         return super().seek(cookie, whence)
-    
+
     def tell(self) -> int:
         if not self.seekable():
             raise IOError("File not open in seekable mode.")
         return super().tell()
-    
 
-    def flush(self):
+    def flush(self) -> None:
         if not self.writable():
             raise IOError("File not open in write mode.")
         super().flush()
         api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files/add(url='{self._filename}', overwrite=true)"
 
         file_size = len(super().getvalue())
         post_request = {
             "Content-Length": str(file_size),
             "X-HTTP-Method": "PUT",
         }
 
         post_request.update(self._header)
         file_content = super().getvalue()
         requests.put(api_url, data=file_content, headers=post_request)
-            
-    def check_back_in(self):
+
+    def check_back_in(self) -> None:
         if self._checkout:
             api_url = f"{self._site}/_api/web/GetFolderByServerRelativeUrl('{self._path}')/Files('{self._filename}')/CheckIn(comment='Comment',checkintype=0)"
             requests.post(api_url, headers=self._header)
 
-    def close(self):
+    def close(self) -> None:
         self.check_back_in()
-        
+
         if self.writable():
             self.flush()
-        
+
         super().close()
-    
+
     def readable(self) -> bool:
         if self._mode != "wb":
             return True
         else:
             return False
 
     def writable(self) -> bool:
         if self._mode != "rb":
             return True
         else:
             return False
-    
+
     def seekable(self) -> bool:
         if "+" in self._mode:
             return True
         else:
             return False
-    
+
     def __enter__(self):
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
@@ -212,40 +211,40 @@
         file_content = super().getvalue().encode()
         requests.put(api_url, data=file_content, headers=post_request)
 
     def read(self, size=-1):
         if not self.readable():
             raise IOError("File not open in read mode.")
         return super().read(size)
-    
+
     def write(self, bytes):
         if not self.writable():
             raise IOError("File not open in write mode.")
         return super().write(bytes)
-    
+
     def truncate(self, __size: int | None = ...) -> int:
-            if not self.seekable():
-                raise IOError("File not open in seekable mode.")
-            return super().truncate(__size)
-    
+        if not self.seekable():
+            raise IOError("File not open in seekable mode.")
+        return super().truncate(__size)
+
     def readline(self, size: int = -1) -> str:
         if not self.readable():
             raise IOError("File not open in read mode.")
         return super().readline(size)
-    
+
     def readlines(self, size: int = -1) -> list[str]:
         if not self.readable():
             raise IOError("File not open in read mode.")
         return super().readlines(size)
-    
+
     def seek(self, cookie: int, whence: int = 0) -> int:
         if not self.seekable():
             raise IOError("File not open in seekable mode.")
         return super().seek(cookie, whence)
-    
+
     def tell(self) -> int:
         if not self.seekable():
             raise IOError("File not open in seekable mode.")
         return super().tell()
 
     def check_back_in(self):
         if self._checkout:
@@ -253,27 +252,27 @@
             requests.post(api_url, headers=self._header)
 
     def close(self):
         self.check_back_in()
         if self.writable():
             self.flush()
         super().close()
-    
+
     def readable(self) -> bool:
         if self._mode != "w":
             return True
         else:
             return False
 
     def writable(self) -> bool:
         if self._mode != "r":
             return True
         else:
             return False
-    
+
     def seekable(self) -> bool:
         if "+" in self._mode:
             return True
         else:
             return False
 
     def __enter__(self):
@@ -282,8 +281,7 @@
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         super().__exit__(exc_type, exc_val, exc_tb)
-
```

### Comparing `sharkpoint-2.0.2/PKG-INFO` & `sharkpoint-3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sharkpoint
-Version: 2.0.2
+Version: 3.0
 Summary: A small Pythonic library for interacting with SharePoint document libraries
 Author: TheOtherOne
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

