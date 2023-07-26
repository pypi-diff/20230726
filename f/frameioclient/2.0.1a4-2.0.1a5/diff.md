# Comparing `tmp/frameioclient-2.0.1a4.tar.gz` & `tmp/frameioclient-2.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frameioclient-2.0.1a4.tar", max compression
+gzip compressed data, was "frameioclient-2.0.1a5.tar", max compression
```

## Comparing `frameioclient-2.0.1a4.tar` & `frameioclient-2.0.1a5.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     1084 2022-08-19 17:13:32.236018 frameioclient-2.0.1a4/LICENSE
--rw-r--r--   0        0        0     3722 2022-08-19 17:13:32.238406 frameioclient-2.0.1a4/README.md
--rw-r--r--   0        0        0       78 2022-08-19 17:13:32.262701 frameioclient-2.0.1a4/frameioclient/__init__.py
--rw-r--r--   0        0        0     1713 2022-08-19 17:13:32.263350 frameioclient-2.0.1a4/frameioclient/client.py
--rw-r--r--   0        0        0      107 2022-08-19 17:13:32.263616 frameioclient-2.0.1a4/frameioclient/config.py
--rw-r--r--   0        0        0     2584 2022-08-19 17:13:32.264281 frameioclient-2.0.1a4/frameioclient/fiocli.py
--rw-r--r--   0        0        0      338 2022-08-19 17:13:32.264934 frameioclient-2.0.1a4/frameioclient/lib/__init__.py
--rw-r--r--   0        0        0      677 2022-08-19 17:13:32.265816 frameioclient-2.0.1a4/frameioclient/lib/constants.py
--rw-r--r--   0        0        0     6112 2022-08-19 17:13:32.266333 frameioclient-2.0.1a4/frameioclient/lib/download.py
--rw-r--r--   0        0        0     2098 2022-08-19 17:13:32.267261 frameioclient-2.0.1a4/frameioclient/lib/exceptions.py
--rw-r--r--   0        0        0      297 2022-08-19 17:13:32.268218 frameioclient-2.0.1a4/frameioclient/lib/logger.py
--rw-r--r--   0        0        0      352 2022-08-19 17:13:32.269203 frameioclient-2.0.1a4/frameioclient/lib/service.py
--rw-r--r--   0        0        0     2599 2022-08-19 17:13:32.270119 frameioclient-2.0.1a4/frameioclient/lib/telemetry.py
--rw-r--r--   0        0        0    15119 2022-08-19 17:13:32.270867 frameioclient-2.0.1a4/frameioclient/lib/transfer.py
--rw-r--r--   0        0        0     6490 2023-03-15 00:48:23.212599 frameioclient-2.0.1a4/frameioclient/lib/transport.py
--rw-r--r--   0        0        0     5193 2023-03-15 00:49:16.404998 frameioclient-2.0.1a4/frameioclient/lib/upload.py
--rw-r--r--   0        0        0     7379 2022-08-19 17:13:32.273002 frameioclient-2.0.1a4/frameioclient/lib/utils.py
--rw-r--r--   0        0        0      275 2022-08-19 17:13:32.273585 frameioclient-2.0.1a4/frameioclient/lib/version.py
--rw-r--r--   0        0        0      273 2022-08-19 17:13:32.274408 frameioclient-2.0.1a4/frameioclient/resources/__init__.py
--rw-r--r--   0        0        0    12805 2023-03-15 00:49:14.591238 frameioclient-2.0.1a4/frameioclient/resources/assets.py
--rw-r--r--   0        0        0     3606 2022-08-19 17:13:32.275639 frameioclient-2.0.1a4/frameioclient/resources/comments.py
--rw-r--r--   0        0        0     5648 2022-08-19 17:13:32.275968 frameioclient-2.0.1a4/frameioclient/resources/helpers.py
--rw-r--r--   0        0        0     3890 2023-03-15 00:48:23.212479 frameioclient-2.0.1a4/frameioclient/resources/links.py
--rw-r--r--   0        0        0      615 2022-08-19 17:13:32.277260 frameioclient-2.0.1a4/frameioclient/resources/logs.py
--rw-r--r--   0        0        0     4657 2022-08-19 17:13:32.278473 frameioclient-2.0.1a4/frameioclient/resources/projects.py
--rw-r--r--   0        0        0     3538 2022-08-19 17:18:30.041949 frameioclient-2.0.1a4/frameioclient/resources/search.py
--rw-r--r--   0        0        0     3123 2023-03-15 00:48:23.212364 frameioclient-2.0.1a4/frameioclient/resources/teams.py
--rw-r--r--   0        0        0      373 2022-08-19 17:13:32.280535 frameioclient-2.0.1a4/frameioclient/resources/users.py
--rw-r--r--   0        0        0     1866 2023-03-15 00:51:01.665038 frameioclient-2.0.1a4/pyproject.toml
--rw-r--r--   0        0        0     4883 2023-03-15 00:51:38.378919 frameioclient-2.0.1a4/setup.py
--rw-r--r--   0        0        0     4903 2023-03-15 00:51:38.379222 frameioclient-2.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-08-19 17:13:32.236018 frameioclient-2.0.1a5/LICENSE
+-rw-r--r--   0        0        0     4193 2023-07-25 23:56:05.448584 frameioclient-2.0.1a5/README.md
+-rw-r--r--   0        0        0       78 2022-08-19 17:13:32.262701 frameioclient-2.0.1a5/frameioclient/__init__.py
+-rw-r--r--   0        0        0     1713 2022-08-19 17:13:32.263350 frameioclient-2.0.1a5/frameioclient/client.py
+-rw-r--r--   0        0        0      107 2022-08-19 17:13:32.263616 frameioclient-2.0.1a5/frameioclient/config.py
+-rw-r--r--   0        0        0     2584 2022-08-19 17:13:32.264281 frameioclient-2.0.1a5/frameioclient/fiocli.py
+-rw-r--r--   0        0        0      338 2022-08-19 17:13:32.264934 frameioclient-2.0.1a5/frameioclient/lib/__init__.py
+-rw-r--r--   0        0        0      677 2022-08-19 17:13:32.265816 frameioclient-2.0.1a5/frameioclient/lib/constants.py
+-rw-r--r--   0        0        0     6112 2022-08-19 17:13:32.266333 frameioclient-2.0.1a5/frameioclient/lib/download.py
+-rw-r--r--   0        0        0     2098 2022-08-19 17:13:32.267261 frameioclient-2.0.1a5/frameioclient/lib/exceptions.py
+-rw-r--r--   0        0        0      297 2022-08-19 17:13:32.268218 frameioclient-2.0.1a5/frameioclient/lib/logger.py
+-rw-r--r--   0        0        0      352 2022-08-19 17:13:32.269203 frameioclient-2.0.1a5/frameioclient/lib/service.py
+-rw-r--r--   0        0        0     2599 2022-08-19 17:13:32.270119 frameioclient-2.0.1a5/frameioclient/lib/telemetry.py
+-rw-r--r--   0        0        0    15119 2022-08-19 17:13:32.270867 frameioclient-2.0.1a5/frameioclient/lib/transfer.py
+-rw-r--r--   0        0        0     6602 2023-07-26 00:03:34.208600 frameioclient-2.0.1a5/frameioclient/lib/transport.py
+-rw-r--r--   0        0        0     5193 2023-03-15 00:49:16.404998 frameioclient-2.0.1a5/frameioclient/lib/upload.py
+-rw-r--r--   0        0        0     7490 2023-07-26 00:03:21.937368 frameioclient-2.0.1a5/frameioclient/lib/utils.py
+-rw-r--r--   0        0        0      275 2022-08-19 17:13:32.273585 frameioclient-2.0.1a5/frameioclient/lib/version.py
+-rw-r--r--   0        0        0      273 2022-08-19 17:13:32.274408 frameioclient-2.0.1a5/frameioclient/resources/__init__.py
+-rw-r--r--   0        0        0    12805 2023-03-15 00:49:14.591238 frameioclient-2.0.1a5/frameioclient/resources/assets.py
+-rw-r--r--   0        0        0     3606 2022-08-19 17:13:32.275639 frameioclient-2.0.1a5/frameioclient/resources/comments.py
+-rw-r--r--   0        0        0     5648 2022-08-19 17:13:32.275968 frameioclient-2.0.1a5/frameioclient/resources/helpers.py
+-rw-r--r--   0        0        0     4513 2023-07-25 23:56:33.041809 frameioclient-2.0.1a5/frameioclient/resources/links.py
+-rw-r--r--   0        0        0      615 2022-08-19 17:13:32.277260 frameioclient-2.0.1a5/frameioclient/resources/logs.py
+-rw-r--r--   0        0        0     4657 2022-08-19 17:13:32.278473 frameioclient-2.0.1a5/frameioclient/resources/projects.py
+-rw-r--r--   0        0        0     3538 2022-08-19 17:18:30.041949 frameioclient-2.0.1a5/frameioclient/resources/search.py
+-rw-r--r--   0        0        0     3194 2023-07-25 23:56:33.042668 frameioclient-2.0.1a5/frameioclient/resources/teams.py
+-rw-r--r--   0        0        0      373 2022-08-19 17:13:32.280535 frameioclient-2.0.1a5/frameioclient/resources/users.py
+-rw-r--r--   0        0        0     1893 2023-07-26 00:08:00.281778 frameioclient-2.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 frameioclient-2.0.1a5/PKG-INFO
```

### Comparing `frameioclient-2.0.1a4/LICENSE` & `frameioclient-2.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/README.md` & `frameioclient-2.0.1a5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,118 +9,123 @@
 # Frame.io 
 Frame.io is a cloud-based collaboration hub that allows video professionals to share files, comment on clips real-time, and compare different versions and edits of a clip. 
 
 ## Overview
 
 ### Installation
 
-via Pip
-```
+via `pip`
+```sh
 $ pip install frameioclient
 ```
 
-via Source
-```
-$ git clone https://github.com/frameio/python-frameio-client
-$ pip install .
-```
-
-### Developing
-Install the package into your development environment and link to it by running the following:
-
+from source
 ```sh
-pipenv install -e . -pre
+$ git clone https://github.com/frameio/python-frameio-client
+$ pip install -e .
 ```
 
 ## Documentation
 
 [Frame.io API Documentation](https://developer.frame.io/docs)
 
 ### Use CLI
-When you install this package, a cli tool called `fioctl` will also be installed to your environment.
+When you install this package, a cli tool called `fioctfioclil` will also be installed to your environment.
 
 **To upload a file or folder**
 ```sh
-fioctl \
+fiocli \
 --token fio-u-YOUR_TOKEN_HERE  \
 --destination "YOUR TARGET FRAME.IO PROJECT OR FOLDER" \
 --target "YOUR LOCAL SYSTEM DIRECTORY" \
 --threads 8
 ```
 
 **To download a file, project, or folder**
 ```sh
-fioctl \
+fiocli \
 --token fio-u-YOUR_TOKEN_HERE  \
 --destination "YOUR LOCAL SYSTEM DIRECTORY" \
 --target "YOUR TARGET FRAME.IO PROJECT OR FOLDER" \
 --threads 2
 ```
 
-### Links
-
-**Sphinx Documentation**
-- https://pythonhosted.org/sphinxcontrib-restbuilder/
-- https://www.npmjs.com/package/rst-selector-parser
-- https://sphinx-themes.org/sample-sites/furo/_sources/index.rst.txt
-- https://developer.mantidproject.org/Standards/DocumentationGuideForDevs.html
-- https://sublime-and-sphinx-guide.readthedocs.io/en/latest/code_blocks.html
-- https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html
-- https://stackoverflow.com/questions/64451966/python-sphinx-how-to-embed-code-into-a-docstring
-- https://pythonhosted.org/an_example_pypi_project/sphinx.html
-
-**Decorators**
-- https://docs.python.org/3.7/library/functools.html
-- https://realpython.com/primer-on-python-decorators/
-- https://www.sphinx-doc.org/en/master/usage/quickstart.html
-- https://www.geeksforgeeks.org/decorators-with-parameters-in-python/
-- https://stackoverflow.com/questions/43544954/why-does-sphinx-autodoc-output-a-decorators-docstring-when-there-are-two-decora
-
-
 ## Usage
 
 _Note: A valid token is required to make requests to Frame.io. Go to our [Developer Portal](https://developer.frame.io/) to get a token!_
 
 In addition to the snippets below, examples are included in [/examples](/examples).
 
 ### Get User Info
 
 Get basic info on the authenticated user.
 
 ```python
+import os
 from frameioclient import FrameioClient
 
-client = FrameioClient("TOKEN")
+# We always recommend passing the token you'll be using via an environment variable and accessing it using os.getenv("FRAMEIO_TOKEN")
+FRAMEIO_TOKEN = os.getenv("FRAMEIO_TOKEN")
+client = FrameioClient(FRAMEIO_TOKEN)
+
 me = client.users.get_me()
 print(me['id'])
 ```
 
 ### Create and Upload Asset
 
 Create a new asset and upload a file. For `parent_asset_id` you must have the root asset ID for the project, or an ID for a folder in the project. For more information on how assets work, check out [our docs](https://developer.frame.io/docs/workflows-assets/uploading-assets).
 
 ```python
 import os
 from frameioclient import FrameioClient
 
-client = FrameioClient("TOKEN")
+# We always recommend passing the token you'll be using via an environment variable and accessing it using os.getenv("FRAMEIO_TOKEN")
+FRAMEIO_TOKEN = os.getenv("FRAMEIO_TOKEN")
+client = FrameioClient(FRAMEIO_TOKEN)
 
 
 # Create a new asset manually
-asset = client.assets.create(
-  parent_asset_id="1234abcd",
+client.assets.create(
+  parent_asset_id="0d98e024-d738-4d9a-ae89-19f02839116d",
   name="MyVideo.mp4",
   type="file",
   filetype="video/mp4",
   filesize=os.path.getsize("sample.mp4")
 )
 
 # Create a new folder
-client.assets.create(
-  parent_asset_id="",
+client.assets.create_folder(
+  parent_asset_id="63bfd7cc-8517-4a61-b655-0a59f5dec630",
   name="Folder name",
-  type="folder" # this kwarg is what makes it a folder
 )
 
 # Upload a file 
 client.assets.upload(destination_id, "video.mp4")
 ```
+
+### Contributing
+Install the package into your development environment using Poetry. This should auto-link it within the current virtual-env that gets created during installation.
+
+```sh
+poetry install
+```
+
+### Ancillary links
+
+**Sphinx Documentation**
+- https://pythonhosted.org/sphinxcontrib-restbuilder/
+- https://www.npmjs.com/package/rst-selector-parser
+- https://sphinx-themes.org/sample-sites/furo/_sources/index.rst.txt
+- https://developer.mantidproject.org/Standards/DocumentationGuideForDevs.html
+- https://sublime-and-sphinx-guide.readthedocs.io/en/latest/code_blocks.html
+- https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html
+- https://stackoverflow.com/questions/64451966/python-sphinx-how-to-embed-code-into-a-docstring
+- https://pythonhosted.org/an_example_pypi_project/sphinx.html
+
+**Decorators**
+- https://docs.python.org/3.7/library/functools.html
+- https://realpython.com/primer-on-python-decorators/
+- https://www.sphinx-doc.org/en/master/usage/quickstart.html
+- https://www.geeksforgeeks.org/decorators-with-parameters-in-python/
+- https://stackoverflow.com/questions/43544954/why-does-sphinx-autodoc-output-a-decorators-docstring-when-there-are-two-decora
+
```

### Comparing `frameioclient-2.0.1a4/frameioclient/client.py` & `frameioclient-2.0.1a5/frameioclient/client.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/fiocli.py` & `frameioclient-2.0.1a5/frameioclient/fiocli.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/lib/constants.py` & `frameioclient-2.0.1a5/frameioclient/lib/constants.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/lib/download.py` & `frameioclient-2.0.1a5/frameioclient/lib/download.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/lib/exceptions.py` & `frameioclient-2.0.1a5/frameioclient/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/lib/telemetry.py` & `frameioclient-2.0.1a5/frameioclient/lib/telemetry.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/lib/transfer.py` & `frameioclient-2.0.1a5/frameioclient/lib/transfer.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/lib/transport.py` & `frameioclient-2.0.1a5/frameioclient/lib/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         # Setup number of threads to use
         self.threads = threads
 
         # Initialize empty thread object
         self.thread_local = None
         self.client_version = ClientVersion.version()
         self.shared_headers = {"x-frameio-client": f"python/{self.client_version}"}
+        self.rate_limit_bypass_header = {"x-client-type": "Socket Service v2"}
 
         # Configure retry strategy (very broad right now)
         self.retry_strategy = Retry(
             total=100,
             backoff_factor=2,
             status_forcelist=retryable_statuses,
             method_whitelist=["GET", "POST", "PUT", "GET", "DELETE"],
@@ -90,15 +91,15 @@
 
     def _format_api_call(self, endpoint: str):
         return f"{self.host}/v2{endpoint}"
 
     def _api_call(
         self, method, endpoint: str, payload: Dict = {}, limit: Optional[int] = None
     ) -> Union[Dict, PaginatedResponse, None]:
-        headers = {**self.shared_headers, **self.auth_header}
+        headers = {**self.shared_headers, **self.auth_header, **self.rate_limit_bypass_header}
 
         r = self.session.request(
             method, self._format_api_call(endpoint), headers=headers, json=payload
         )
 
         if r.ok:
             if r.headers.get("page-number"):
```

### Comparing `frameioclient-2.0.1a4/frameioclient/lib/upload.py` & `frameioclient-2.0.1a5/frameioclient/lib/upload.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/lib/utils.py` & `frameioclient-2.0.1a5/frameioclient/lib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,19 @@
         Example::
         
             stream(lambda pagination: client.get_collaborators(project_id, **pagination))
         """
         total_pages = page
         while page <= total_pages:
             result_list = func(page=page, page_size=page_size)
-            total_pages = result_list.total_pages
-            for res in result_list:
+            if type(result_list) == PaginatedResponse:
+                total_pages = result_list.total_pages
+                for res in result_list:
+                    yield res
+            else:
                 yield res
 
             page += 1
 
     @staticmethod
     def stream_results(
         endpoint, page=1, page_size=50, client=None, **_kwargs
```

### Comparing `frameioclient-2.0.1a4/frameioclient/resources/assets.py` & `frameioclient-2.0.1a5/frameioclient/resources/assets.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/resources/comments.py` & `frameioclient-2.0.1a5/frameioclient/resources/comments.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/resources/helpers.py` & `frameioclient-2.0.1a5/frameioclient/resources/helpers.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/resources/links.py` & `frameioclient-2.0.1a5/frameioclient/resources/links.py`

 * *Files 8% similar despite different names*

```diff
@@ -130,7 +130,28 @@
             asset_id="9cee7966-4066-b326-7db1-f9e6f5e929e4",
             title="My fresh presentation",
             password="abc123"
           )
         """
         endpoint = "/assets/{}/presentations".format(asset_id)
         return self.client._api_call("post", endpoint, payload=kwargs)
+
+    def update(self, presentation_id: Union[str, UUID], **kwargs):
+        """
+        Update a presentation link.
+
+        Args:
+          presentation_id (string): The presentation id.
+
+        :Keyword Arguments:
+          kwargs: additional request parameters.
+
+        Example::
+
+          client.presentation_links.update(
+            presentation_id="9cee7966-4066-b326-7db1-f9e6f5e929e4",
+            name="My fresh presentation",
+            enabled=False
+          )
+        """
+        endpoint = "/presentations/{}".format(presentation_id)
+        return self.client._api_call("put", endpoint, payload=kwargs)
```

### Comparing `frameioclient-2.0.1a4/frameioclient/resources/logs.py` & `frameioclient-2.0.1a5/frameioclient/resources/logs.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/resources/projects.py` & `frameioclient-2.0.1a5/frameioclient/resources/projects.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/resources/search.py` & `frameioclient-2.0.1a5/frameioclient/resources/search.py`

 * *Files identical despite different names*

### Comparing `frameioclient-2.0.1a4/frameioclient/resources/teams.py` & `frameioclient-2.0.1a5/frameioclient/resources/teams.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,12 +94,14 @@
         Remove a list of users via their e-mail address from a given team.
 
         Args:
             team_id (string): The team id.
             emails (list): The e-mails you want to add.
         """
 
+        # TODO: Implement pagination here since the batch size is 20?
+
         payload = dict()
         payload["batch"] = list(map(lambda email: {"email": email}, emails))
 
         endpoint = "/batch/teams/{}/members".format(team_id)
         return self.client._api_call("delete", endpoint, payload=payload)
```

### Comparing `frameioclient-2.0.1a4/pyproject.toml` & `frameioclient-2.0.1a5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frameioclient"
-version = "2.0.1-alpha.4"
+version = "2.0.1a5"
 description='Client library for the Frame.io API'
 readme = "README.md"
 license='MIT'
 homepage = "https://github.com/Frameio/python-frameio-client"
 authors = ["Frame.io DevRel <platform@frame.io>"]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
@@ -23,14 +23,16 @@
 analytics-python = "^1.4.0"
 enlighten = "^1.10.2"
 importlib-metadata = "^4.11.3"
 requests = "^2.27.1"
 token-bucket = "^0.3.0"
 urllib3 = "^1.26.9"
 xxhash = "^3.0.0"
+furl = "^2.1.3"
+tqdm = "^4.64.1"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
 
 # Optional dependencies
 Sphinx = { version = "^4.4.0", optional = true }
 sphinx-jekyll-builder = { version = "^0.3.0", optional = true }
```

### Comparing `frameioclient-2.0.1a4/PKG-INFO` & `frameioclient-2.0.1a5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 Metadata-Version: 2.1
 Name: frameioclient
-Version: 2.0.1a4
+Version: 2.0.1a5
 Summary: Client library for the Frame.io API
 Home-page: https://github.com/Frameio/python-frameio-client
 License: MIT
 Author: Frame.io DevRel
 Author-email: platform@frame.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: analytics-python (>=1.4.0,<2.0.0)
 Requires-Dist: enlighten (>=1.10.2,<2.0.0)
+Requires-Dist: furl (>=2.1.3,<3.0.0)
 Requires-Dist: importlib-metadata (>=4.11.3,<5.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: token-bucket (>=0.3.0,<0.4.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.9,<2.0.0)
 Requires-Dist: xxhash (>=3.0.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # python-frameio-client
 
 [![PyPI version](https://badge.fury.io/py/frameioclient.svg)](https://badge.fury.io/py/frameioclient)
@@ -39,119 +45,124 @@
 # Frame.io 
 Frame.io is a cloud-based collaboration hub that allows video professionals to share files, comment on clips real-time, and compare different versions and edits of a clip. 
 
 ## Overview
 
 ### Installation
 
-via Pip
-```
+via `pip`
+```sh
 $ pip install frameioclient
 ```
 
-via Source
-```
-$ git clone https://github.com/frameio/python-frameio-client
-$ pip install .
-```
-
-### Developing
-Install the package into your development environment and link to it by running the following:
-
+from source
 ```sh
-pipenv install -e . -pre
+$ git clone https://github.com/frameio/python-frameio-client
+$ pip install -e .
 ```
 
 ## Documentation
 
 [Frame.io API Documentation](https://developer.frame.io/docs)
 
 ### Use CLI
-When you install this package, a cli tool called `fioctl` will also be installed to your environment.
+When you install this package, a cli tool called `fioctfioclil` will also be installed to your environment.
 
 **To upload a file or folder**
 ```sh
-fioctl \
+fiocli \
 --token fio-u-YOUR_TOKEN_HERE  \
 --destination "YOUR TARGET FRAME.IO PROJECT OR FOLDER" \
 --target "YOUR LOCAL SYSTEM DIRECTORY" \
 --threads 8
 ```
 
 **To download a file, project, or folder**
 ```sh
-fioctl \
+fiocli \
 --token fio-u-YOUR_TOKEN_HERE  \
 --destination "YOUR LOCAL SYSTEM DIRECTORY" \
 --target "YOUR TARGET FRAME.IO PROJECT OR FOLDER" \
 --threads 2
 ```
 
-### Links
-
-**Sphinx Documentation**
-- https://pythonhosted.org/sphinxcontrib-restbuilder/
-- https://www.npmjs.com/package/rst-selector-parser
-- https://sphinx-themes.org/sample-sites/furo/_sources/index.rst.txt
-- https://developer.mantidproject.org/Standards/DocumentationGuideForDevs.html
-- https://sublime-and-sphinx-guide.readthedocs.io/en/latest/code_blocks.html
-- https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html
-- https://stackoverflow.com/questions/64451966/python-sphinx-how-to-embed-code-into-a-docstring
-- https://pythonhosted.org/an_example_pypi_project/sphinx.html
-
-**Decorators**
-- https://docs.python.org/3.7/library/functools.html
-- https://realpython.com/primer-on-python-decorators/
-- https://www.sphinx-doc.org/en/master/usage/quickstart.html
-- https://www.geeksforgeeks.org/decorators-with-parameters-in-python/
-- https://stackoverflow.com/questions/43544954/why-does-sphinx-autodoc-output-a-decorators-docstring-when-there-are-two-decora
-
-
 ## Usage
 
 _Note: A valid token is required to make requests to Frame.io. Go to our [Developer Portal](https://developer.frame.io/) to get a token!_
 
 In addition to the snippets below, examples are included in [/examples](/examples).
 
 ### Get User Info
 
 Get basic info on the authenticated user.
 
 ```python
+import os
 from frameioclient import FrameioClient
 
-client = FrameioClient("TOKEN")
+# We always recommend passing the token you'll be using via an environment variable and accessing it using os.getenv("FRAMEIO_TOKEN")
+FRAMEIO_TOKEN = os.getenv("FRAMEIO_TOKEN")
+client = FrameioClient(FRAMEIO_TOKEN)
+
 me = client.users.get_me()
 print(me['id'])
 ```
 
 ### Create and Upload Asset
 
 Create a new asset and upload a file. For `parent_asset_id` you must have the root asset ID for the project, or an ID for a folder in the project. For more information on how assets work, check out [our docs](https://developer.frame.io/docs/workflows-assets/uploading-assets).
 
 ```python
 import os
 from frameioclient import FrameioClient
 
-client = FrameioClient("TOKEN")
+# We always recommend passing the token you'll be using via an environment variable and accessing it using os.getenv("FRAMEIO_TOKEN")
+FRAMEIO_TOKEN = os.getenv("FRAMEIO_TOKEN")
+client = FrameioClient(FRAMEIO_TOKEN)
 
 
 # Create a new asset manually
-asset = client.assets.create(
-  parent_asset_id="1234abcd",
+client.assets.create(
+  parent_asset_id="0d98e024-d738-4d9a-ae89-19f02839116d",
   name="MyVideo.mp4",
   type="file",
   filetype="video/mp4",
   filesize=os.path.getsize("sample.mp4")
 )
 
 # Create a new folder
-client.assets.create(
-  parent_asset_id="",
+client.assets.create_folder(
+  parent_asset_id="63bfd7cc-8517-4a61-b655-0a59f5dec630",
   name="Folder name",
-  type="folder" # this kwarg is what makes it a folder
 )
 
 # Upload a file 
 client.assets.upload(destination_id, "video.mp4")
 ```
 
+### Contributing
+Install the package into your development environment using Poetry. This should auto-link it within the current virtual-env that gets created during installation.
+
+```sh
+poetry install
+```
+
+### Ancillary links
+
+**Sphinx Documentation**
+- https://pythonhosted.org/sphinxcontrib-restbuilder/
+- https://www.npmjs.com/package/rst-selector-parser
+- https://sphinx-themes.org/sample-sites/furo/_sources/index.rst.txt
+- https://developer.mantidproject.org/Standards/DocumentationGuideForDevs.html
+- https://sublime-and-sphinx-guide.readthedocs.io/en/latest/code_blocks.html
+- https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html
+- https://stackoverflow.com/questions/64451966/python-sphinx-how-to-embed-code-into-a-docstring
+- https://pythonhosted.org/an_example_pypi_project/sphinx.html
+
+**Decorators**
+- https://docs.python.org/3.7/library/functools.html
+- https://realpython.com/primer-on-python-decorators/
+- https://www.sphinx-doc.org/en/master/usage/quickstart.html
+- https://www.geeksforgeeks.org/decorators-with-parameters-in-python/
+- https://stackoverflow.com/questions/43544954/why-does-sphinx-autodoc-output-a-decorators-docstring-when-there-are-two-decora
+
+
```

