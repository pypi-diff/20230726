# Comparing `tmp/openi-beta-2.0.2.tar.gz` & `tmp/openi-beta-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-2.0.2.tar", last modified: Mon Jul 24 09:36:03 2023, max compression
+gzip compressed data, was "openi-beta-2.0.3.tar", last modified: Wed Jul 26 01:34:23 2023, max compression
```

## Comparing `openi-beta-2.0.2.tar` & `openi-beta-2.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.871833 openi-beta-2.0.2/
--rw-rw-rw-   0        0        0     5381 2023-07-24 09:36:03.871833 openi-beta-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4735 2023-07-24 07:49:31.000000 openi-beta-2.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 09:36:03.872833 openi-beta-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-07-24 09:35:46.000000 openi-beta-2.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.840204 openi-beta-2.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.846206 openi-beta-2.0.2/src/openi/
--rw-rw-rw-   0        0        0      194 2023-07-24 07:15:17.000000 openi-beta-2.0.2/src/openi/__init__.py
--rw-rw-rw-   0        0        0     6459 2023-07-24 07:13:05.000000 openi-beta-2.0.2/src/openi/apis.py
--rw-rw-rw-   0        0        0     5238 2023-07-24 07:13:04.000000 openi-beta-2.0.2/src/openi/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.850204 openi-beta-2.0.2/src/openi/cloudbrain/
--rw-rw-rw-   0        0        0       84 2023-07-24 07:06:23.000000 openi-beta-2.0.2/src/openi/cloudbrain/__init__.py
--rw-rw-rw-   0        0        0     1609 2023-07-24 07:06:26.000000 openi-beta-2.0.2/src/openi/cloudbrain/env_check.py
--rw-rw-rw-   0        0        0     5313 2023-07-24 07:06:29.000000 openi-beta-2.0.2/src/openi/cloudbrain/helper.py
--rw-rw-rw-   0        0        0     1559 2023-07-24 07:06:31.000000 openi-beta-2.0.2/src/openi/cloudbrain/minio_operate.py
--rw-rw-rw-   0        0        0     2886 2023-07-24 07:06:32.000000 openi-beta-2.0.2/src/openi/cloudbrain/obs_operate.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.853204 openi-beta-2.0.2/src/openi/dataset/
--rw-rw-rw-   0        0        0      109 2023-07-24 07:06:34.000000 openi-beta-2.0.2/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0     2855 2023-07-24 07:06:35.000000 openi-beta-2.0.2/src/openi/dataset/dataset_file.py
--rw-rw-rw-   0        0        0     2685 2023-07-24 07:20:32.000000 openi-beta-2.0.2/src/openi/dataset/download.py
--rw-rw-rw-   0        0        0     4669 2023-07-24 09:18:26.000000 openi-beta-2.0.2/src/openi/dataset/upload.py
--rw-rw-rw-   0        0        0     3356 2023-07-24 07:13:03.000000 openi-beta-2.0.2/src/openi/login.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.855203 openi-beta-2.0.2/src/openi/path/
--rw-rw-rw-   0        0        0       21 2023-07-24 07:06:52.000000 openi-beta-2.0.2/src/openi/path/__init__.py
--rw-rw-rw-   0        0        0     2405 2023-07-24 07:07:00.000000 openi-beta-2.0.2/src/openi/path/path.py
--rw-rw-rw-   0        0        0     4081 2023-07-24 09:33:32.000000 openi-beta-2.0.2/src/openi/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.857203 openi-beta-2.0.2/src/openi/utils/
--rw-rw-rw-   0        0        0       50 2023-07-24 07:07:03.000000 openi-beta-2.0.2/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     2197 2023-07-24 07:07:05.000000 openi-beta-2.0.2/src/openi/utils/file_utils.py
--rw-rw-rw-   0        0        0      723 2023-07-24 07:07:16.000000 openi-beta-2.0.2/src/openi/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.869833 openi-beta-2.0.2/src/openi_beta.egg-info/
--rw-rw-rw-   0        0        0     5381 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 09:36:03.000000 openi-beta-2.0.2/src/openi_beta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 09:36:03.870832 openi-beta-2.0.2/test/
--rw-rw-rw-   0        0        0       87 2023-07-24 07:35:25.000000 openi-beta-2.0.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:34:23.748183 openi-beta-2.0.3/
+-rw-rw-rw-   0        0        0     5381 2023-07-26 01:34:23.747079 openi-beta-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4735 2023-07-24 07:49:31.000000 openi-beta-2.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 01:34:23.748183 openi-beta-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-07-26 01:33:57.000000 openi-beta-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:34:23.728106 openi-beta-2.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 01:34:23.732258 openi-beta-2.0.3/src/openi/
+-rw-rw-rw-   0        0        0      194 2023-07-26 01:33:14.000000 openi-beta-2.0.3/src/openi/__init__.py
+-rw-rw-rw-   0        0        0     6456 2023-07-26 01:30:58.000000 openi-beta-2.0.3/src/openi/apis.py
+-rw-rw-rw-   0        0        0     5238 2023-07-26 01:33:22.000000 openi-beta-2.0.3/src/openi/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:34:23.735046 openi-beta-2.0.3/src/openi/cloudbrain/
+-rw-rw-rw-   0        0        0       84 2023-07-24 07:06:23.000000 openi-beta-2.0.3/src/openi/cloudbrain/__init__.py
+-rw-rw-rw-   0        0        0     1609 2023-07-24 07:06:26.000000 openi-beta-2.0.3/src/openi/cloudbrain/env_check.py
+-rw-rw-rw-   0        0        0     5313 2023-07-24 07:06:29.000000 openi-beta-2.0.3/src/openi/cloudbrain/helper.py
+-rw-rw-rw-   0        0        0     1559 2023-07-24 07:06:31.000000 openi-beta-2.0.3/src/openi/cloudbrain/minio_operate.py
+-rw-rw-rw-   0        0        0     2886 2023-07-24 07:06:32.000000 openi-beta-2.0.3/src/openi/cloudbrain/obs_operate.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:34:23.736254 openi-beta-2.0.3/src/openi/dataset/
+-rw-rw-rw-   0        0        0      109 2023-07-24 07:06:34.000000 openi-beta-2.0.3/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2752 2023-07-26 01:32:22.000000 openi-beta-2.0.3/src/openi/dataset/dataset_file.py
+-rw-rw-rw-   0        0        0     2685 2023-07-26 01:32:31.000000 openi-beta-2.0.3/src/openi/dataset/download.py
+-rw-rw-rw-   0        0        0     4379 2023-07-26 01:32:58.000000 openi-beta-2.0.3/src/openi/dataset/upload.py
+-rw-rw-rw-   0        0        0     3029 2023-07-26 01:31:33.000000 openi-beta-2.0.3/src/openi/login.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:34:23.737476 openi-beta-2.0.3/src/openi/path/
+-rw-rw-rw-   0        0        0       21 2023-07-24 07:06:52.000000 openi-beta-2.0.3/src/openi/path/__init__.py
+-rw-rw-rw-   0        0        0     2405 2023-07-26 01:32:02.000000 openi-beta-2.0.3/src/openi/path/path.py
+-rw-rw-rw-   0        0        0     4081 2023-07-26 01:33:29.000000 openi-beta-2.0.3/src/openi/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:34:23.740562 openi-beta-2.0.3/src/openi/utils/
+-rw-rw-rw-   0        0        0       50 2023-07-24 07:07:03.000000 openi-beta-2.0.3/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-07-26 01:31:45.000000 openi-beta-2.0.3/src/openi/utils/file_utils.py
+-rw-rw-rw-   0        0        0      723 2023-07-26 01:33:04.000000 openi-beta-2.0.3/src/openi/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:34:23.746076 openi-beta-2.0.3/src/openi_beta.egg-info/
+-rw-rw-rw-   0        0        0     5381 2023-07-26 01:34:23.000000 openi-beta-2.0.3/src/openi_beta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-07-26 01:34:23.000000 openi-beta-2.0.3/src/openi_beta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 01:34:23.000000 openi-beta-2.0.3/src/openi_beta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-26 01:34:23.000000 openi-beta-2.0.3/src/openi_beta.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-26 01:34:23.000000 openi-beta-2.0.3/src/openi_beta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 01:34:23.000000 openi-beta-2.0.3/src/openi_beta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 01:34:23.747079 openi-beta-2.0.3/test/
+-rw-rw-rw-   0        0        0       87 2023-07-24 07:35:25.000000 openi-beta-2.0.3/test/test.py
```

### Comparing `openi-beta-2.0.2/PKG-INFO` & `openi-beta-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 2.0.2
+Version: 2.0.3
 Summary: Beta package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-2.0.2/README.md` & `openi-beta-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.2/setup.py` & `openi-beta-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="openi-beta",
-    version="2.0.2",
+    version="2.0.3",
     description="Beta package for openi pypi",
     package_dir={"": "src"},
     packages=find_packages("src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
     author="chenzh05",
```

### Comparing `openi-beta-2.0.2/src/openi/apis.py` & `openi-beta-2.0.3/src/openi/apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 """
 APIS
 """
 
 
 class OpeniAPI:
     def __init__(self, endpoint: str = None, token: str = None):
-        self.endpoint = (
-            file_utils.get_token()["endpoint"] + API.VERSION
-            if endpoint is None
-            else endpoint + API.VERSION
+        self.baseURL = (
+            file_utils.get_token()["endpoint"] if endpoint is None else endpoint
         )
+        self.endpoint = self.baseURL + API.VERSION
         self.token = file_utils.get_token()["token"] if token is None else token
 
     def catch_auth_error(self, x):
         if x.status_code == 401:
             msg = f"❌ {x} {x.reason} - failed to connecting OPENI, please check your `token` or permssion."
             logging.error(msg)
             raise PermissionError(msg)
```

### Comparing `openi-beta-2.0.2/src/openi/cli.py` & `openi-beta-2.0.3/src/openi/cli.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.2/src/openi/cloudbrain/env_check.py` & `openi-beta-2.0.3/src/openi/cloudbrain/env_check.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.2/src/openi/cloudbrain/helper.py` & `openi-beta-2.0.3/src/openi/cloudbrain/helper.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.2/src/openi/cloudbrain/minio_operate.py` & `openi-beta-2.0.3/src/openi/cloudbrain/minio_operate.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.2/src/openi/cloudbrain/obs_operate.py` & `openi-beta-2.0.3/src/openi/cloudbrain/obs_operate.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.2/src/openi/dataset/dataset_file.py` & `openi-beta-2.0.3/src/openi/dataset/dataset_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,9 +86,7 @@
         upload_type = DATASET.SOTRAGE_TYPE[cluster]
         cluster = cluster
         return upload_type, cluster
     except:
         msg = f"❌ argument `cluster` must be either `GPU` or `NPU`"
         logging.error(msg)
         raise ValueError(msg)
-        # print("❌ argument `cluster` must be either `GPU` or `NPU`")
-        # raise SystemExit()
```

### Comparing `openi-beta-2.0.2/src/openi/dataset/download.py` & `openi-beta-2.0.3/src/openi/dataset/download.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.2/src/openi/dataset/upload.py` & `openi-beta-2.0.3/src/openi/dataset/upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 logger.setup_logger()
 
 
 def upload_with_tqdm(_file: DatasetFile, api: OpeniAPI, upload_chunks: list):
     chunk_size = _file.chunk_size
     _progress = chunk_size * (_file.total_chunks_count - len(upload_chunks))
-    # _desc = 'Uploading' if _progress == 0 else 'Continue uploading'
 
     with tqdm(
         total=_file.size,
         leave=True,
         initial=_progress,
         unit="B",
         unit_scale=True,
@@ -91,18 +90,15 @@
         else:
             msg = f"❌ Upload failed: {_file.filename}` ({cluster}), please contact us. "
             logging.error(msg)
             raise RuntimeError(msg)
 
     # upload completed
     if _get_chunks["uploaded"] == "1":
-        # if _get_chunks.attachID == "0": # 删除数据集记录，未删除文件
-        #     api.add_attachments(_file) # current not implemented in swagger api
         if _get_chunks["datasetID"] != "" and _get_chunks["datasetName"] != "":
-            # ?on web js: and file.realName != ""
             msg = (
                 f"❌ Upload failed: `{_file.filename}` ({cluster})"
                 " already exists in "
                 f"{api.endpoint.split('/api')[0]}/{_file.owner}/{_get_chunks['repoName']}/datasets"
             )
             logging.error(msg)
             raise ValueError(msg)
```

### Comparing `openi-beta-2.0.2/src/openi/login.py` & `openi-beta-2.0.3/src/openi/login.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,25 +22,19 @@
              ╚═════╝   ╚═╝      ╚══════╝  ╚═╝  ╚═══╝  ╚═════╝\n
          """
     )
     endpoint = endpoint[:-1] if endpoint[-1] == "/" else endpoint
 
     if token is None:
         print(f"点击链接获取令牌并复制粘贴到下列输入栏 {endpoint}/user/settings/applications \n")
-        if os.path.exists(PATH.TOKEN_PATH):
-            # print(f"[WARNING] A token was found on this machine, "
-            #       "enter a new token will overwrite the existing one. "
-            #       "use `whoami` to display username, or `logout` to delete it.\n")
-            print(
-                f"[WARNING] 若本机已存在登录令牌，本次输入的令牌会将其覆盖 \n"
-                "          若粘贴时切换了本窗口，请先按 退格键⇦ 删除多余空格\n"
-            )
+        print(
+            f"[WARNING] 若本机已存在登录令牌，本次输入的令牌会将其覆盖 \n"
+            "          若粘贴时切换了本窗口，请先按 退格键⇦ 删除多余空格\n"
+        )
         token = getpass(prompt="  🔒 token: ")
-        # cli_login(endpoint)
-    # else:
     _login(token=token, endpoint=endpoint)
 
 
 def _login(token: str, endpoint: str) -> None:
     try:
         api = OpeniAPI(endpoint, token)
         valid_user = api.login_check()
@@ -58,16 +52,17 @@
         print(msg)
     except:
         raise ValueError("\n  ❌ login failed: invalid token or endpoint!\n")
 
 
 def whoami() -> None:
     try:
-        valid_user = get_token()
-        msg = f"\n`{valid_user['username']}` @{valid_user['endpoint']}\n"
+        api = OpeniAPI()
+        valid_user = api.login_check()
+        msg = f"\n`{valid_user}` @{api.baseURL}\n"
         logging.info(msg)
         print(msg)
     except:
         msg = f"\nCurrently not logged in.\n"
         logging.info(msg)
         print(msg)
```

### Comparing `openi-beta-2.0.2/src/openi/path/path.py` & `openi-beta-2.0.3/src/openi/path/path.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.2/src/openi/settings.py` & `openi-beta-2.0.3/src/openi/settings.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.2/src/openi/utils/logger.py` & `openi-beta-2.0.3/src/openi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.2/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-2.0.3/src/openi_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 2.0.2
+Version: 2.0.3
 Summary: Beta package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-2.0.2/src/openi_beta.egg-info/SOURCES.txt` & `openi-beta-2.0.3/src/openi_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

