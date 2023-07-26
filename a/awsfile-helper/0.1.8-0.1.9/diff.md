# Comparing `tmp/awsfile-helper-0.1.8.tar.gz` & `tmp/awsfile-helper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsfile-helper-0.1.8.tar", max compression
+gzip compressed data, was "awsfile-helper-0.1.9.tar", max compression
```

## Comparing `awsfile-helper-0.1.8.tar` & `awsfile-helper-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      307 2022-11-01 20:07:25.846675 awsfile-helper-0.1.8/awsfile_helper/__init__.py
--rw-r--r--   0        0        0       54 2022-11-01 20:07:25.841678 awsfile-helper-0.1.8/awsfile_helper/bp/__init__.py
--rw-r--r--   0        0        0     4728 2022-11-01 20:39:39.081713 awsfile-helper-0.1.8/awsfile_helper/bp/aws_api.py
--rw-r--r--   0        0        0      270 2022-11-01 20:07:25.847175 awsfile-helper-0.1.8/awsfile_helper/dmo/__init__.py
--rw-r--r--   0        0        0      989 2022-11-11 22:47:07.394191 awsfile-helper-0.1.8/awsfile_helper/dmo/credential_manager.py
--rw-r--r--   0        0        0      975 2022-11-01 20:08:18.614513 awsfile-helper-0.1.8/awsfile_helper/dmo/file_content_reader.py
--rw-r--r--   0        0        0     1374 2022-11-01 20:55:21.089994 awsfile-helper-0.1.8/awsfile_helper/dmo/file_content_writer.py
--rw-r--r--   0        0        0     1901 2022-11-01 20:08:23.709653 awsfile-helper-0.1.8/awsfile_helper/dmo/s3_bucket_reader.py
--rw-r--r--   0        0        0     1861 2022-11-01 21:55:53.577179 awsfile-helper-0.1.8/awsfile_helper/dmo/s3_image_writer.py
--rw-r--r--   0        0        0     2470 2022-11-01 20:38:35.649495 awsfile-helper-0.1.8/awsfile_helper/find_jpg_file.py
--rw-r--r--   0        0        0     2230 2022-11-01 20:47:58.409322 awsfile-helper-0.1.8/awsfile_helper/find_owl_file.py
--rw-r--r--   0        0        0     6215 2022-11-01 20:46:31.755116 awsfile-helper-0.1.8/awsfile_helper/find_s3_file.py
--rw-r--r--   0        0        0      311 2022-11-01 20:07:25.842176 awsfile-helper-0.1.8/awsfile_helper/svc/__init__.py
--rw-r--r--   0        0        0      807 2022-11-01 20:08:30.842879 awsfile-helper-0.1.8/awsfile_helper/svc/connect_to_s3.py
--rw-r--r--   0        0        0     4709 2022-11-01 21:56:02.328667 awsfile-helper-0.1.8/awsfile_helper/svc/download_from_s3.py
--rw-r--r--   0        0        0     1698 2022-11-01 20:39:49.736974 awsfile-helper-0.1.8/awsfile_helper/svc/find_file_by_version.py
--rw-r--r--   0        0        0     2265 2022-11-01 20:39:56.194640 awsfile-helper-0.1.8/awsfile_helper/svc/find_latest_version_number.py
--rw-r--r--   0        0        0     2061 2022-11-01 21:56:04.819161 awsfile-helper-0.1.8/awsfile_helper/svc/read_from_cache.py
--rw-r--r--   0        0        0     1917 2022-11-01 20:08:46.685248 awsfile-helper-0.1.8/awsfile_helper/svc/read_from_s3.py
--rw-r--r--   0        0        0     1407 2022-11-11 22:48:26.336232 awsfile-helper-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2763 2022-11-01 20:07:24.290677 awsfile-helper-0.1.8/README.md
--rw-r--r--   0        0        0     3538 2022-11-11 22:49:28.318403 awsfile-helper-0.1.8/setup.py
--rw-r--r--   0        0        0     3561 2022-11-11 22:49:28.318902 awsfile-helper-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      307 2022-11-01 20:07:25.846675 awsfile-helper-0.1.9/awsfile_helper/__init__.py
+-rw-r--r--   0        0        0       54 2022-11-01 20:07:25.841678 awsfile-helper-0.1.9/awsfile_helper/bp/__init__.py
+-rw-r--r--   0        0        0     5586 2022-11-12 00:24:11.396524 awsfile-helper-0.1.9/awsfile_helper/bp/aws_api.py
+-rw-r--r--   0        0        0      270 2022-11-01 20:07:25.847175 awsfile-helper-0.1.9/awsfile_helper/dmo/__init__.py
+-rw-r--r--   0        0        0     1966 2022-11-12 00:23:49.658064 awsfile-helper-0.1.9/awsfile_helper/dmo/credential_manager.py
+-rw-r--r--   0        0        0     1278 2022-11-12 00:19:13.825220 awsfile-helper-0.1.9/awsfile_helper/dmo/file_content_reader.py
+-rw-r--r--   0        0        0     1668 2022-11-12 00:19:44.569563 awsfile-helper-0.1.9/awsfile_helper/dmo/file_content_writer.py
+-rw-r--r--   0        0        0     1901 2022-11-01 20:08:23.709653 awsfile-helper-0.1.9/awsfile_helper/dmo/s3_bucket_reader.py
+-rw-r--r--   0        0        0     1861 2022-11-01 21:55:53.577179 awsfile-helper-0.1.9/awsfile_helper/dmo/s3_image_writer.py
+-rw-r--r--   0        0        0     2470 2022-11-01 20:38:35.649495 awsfile-helper-0.1.9/awsfile_helper/find_jpg_file.py
+-rw-r--r--   0        0        0     2230 2022-11-01 20:47:58.409322 awsfile-helper-0.1.9/awsfile_helper/find_owl_file.py
+-rw-r--r--   0        0        0     6215 2022-11-01 20:46:31.755116 awsfile-helper-0.1.9/awsfile_helper/find_s3_file.py
+-rw-r--r--   0        0        0      311 2022-11-01 20:07:25.842176 awsfile-helper-0.1.9/awsfile_helper/svc/__init__.py
+-rw-r--r--   0        0        0     1673 2022-11-12 00:23:41.583349 awsfile-helper-0.1.9/awsfile_helper/svc/connect_to_s3.py
+-rw-r--r--   0        0        0     4709 2022-11-01 21:56:02.328667 awsfile-helper-0.1.9/awsfile_helper/svc/download_from_s3.py
+-rw-r--r--   0        0        0     1698 2022-11-01 20:39:49.736974 awsfile-helper-0.1.9/awsfile_helper/svc/find_file_by_version.py
+-rw-r--r--   0        0        0     2265 2022-11-01 20:39:56.194640 awsfile-helper-0.1.9/awsfile_helper/svc/find_latest_version_number.py
+-rw-r--r--   0        0        0     2061 2022-11-01 21:56:04.819161 awsfile-helper-0.1.9/awsfile_helper/svc/read_from_cache.py
+-rw-r--r--   0        0        0     1917 2022-11-01 20:08:46.685248 awsfile-helper-0.1.9/awsfile_helper/svc/read_from_s3.py
+-rw-r--r--   0        0        0     1407 2022-11-12 00:14:56.146830 awsfile-helper-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2763 2022-11-01 20:07:24.290677 awsfile-helper-0.1.9/README.md
+-rw-r--r--   0        0        0     3538 2022-11-12 00:26:15.062548 awsfile-helper-0.1.9/setup.py
+-rw-r--r--   0        0        0     3561 2022-11-12 00:26:15.063047 awsfile-helper-0.1.9/PKG-INFO
```

### Comparing `awsfile-helper-0.1.8/awsfile_helper/dmo/file_content_writer.py` & `awsfile-helper-0.1.9/awsfile_helper/dmo/file_content_writer.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,14 +24,24 @@
         """
         BaseObject.__init__(self, __name__)
 
     def process(self,
                 file_data: object,
                 file_path: str,
                 file_ext: str) -> None:
+        """ Write Content to File
+
+        Args:
+            file_data (object): the file data
+            file_path (str): the absolute file path
+            file_ext (str): the file extension
+
+        Raises:
+            NotImplementedError: unrecognized file extension
+        """
 
         if not file_data or not len(file_data):
             return None
 
         if file_ext in ['txt', 'owl', 'csv', 'tsv']:
             FileIO.write_string(input_text=file_data,
                                 file_path=file_path)
```

### Comparing `awsfile-helper-0.1.8/awsfile_helper/dmo/s3_bucket_reader.py` & `awsfile-helper-0.1.9/awsfile_helper/dmo/s3_bucket_reader.py`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/awsfile_helper/dmo/s3_image_writer.py` & `awsfile-helper-0.1.9/awsfile_helper/dmo/s3_image_writer.py`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/awsfile_helper/find_jpg_file.py` & `awsfile-helper-0.1.9/awsfile_helper/find_jpg_file.py`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/awsfile_helper/find_owl_file.py` & `awsfile-helper-0.1.9/awsfile_helper/find_owl_file.py`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/awsfile_helper/find_s3_file.py` & `awsfile-helper-0.1.9/awsfile_helper/find_s3_file.py`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/awsfile_helper/svc/download_from_s3.py` & `awsfile-helper-0.1.9/awsfile_helper/svc/download_from_s3.py`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/awsfile_helper/svc/find_file_by_version.py` & `awsfile-helper-0.1.9/awsfile_helper/svc/find_file_by_version.py`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/awsfile_helper/svc/find_latest_version_number.py` & `awsfile-helper-0.1.9/awsfile_helper/svc/find_latest_version_number.py`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/awsfile_helper/svc/read_from_cache.py` & `awsfile-helper-0.1.9/awsfile_helper/svc/read_from_cache.py`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/awsfile_helper/svc/read_from_s3.py` & `awsfile-helper-0.1.9/awsfile_helper/svc/read_from_s3.py`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/pyproject.toml` & `awsfile-helper-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ]
 
 description = "AWS File Helper for Easier I/O"
 license = "None"
 name = "awsfile-helper"
 readme = "README.md"
 
-version = "0.1.8"
+version = "0.1.9"
 
 keywords = ["aws", "cloud", "s3", "bucket", "helper", "utility"]
 repository = "https://github.com/craigtrim/awsfile-helper"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `awsfile-helper-0.1.8/README.md` & `awsfile-helper-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `awsfile-helper-0.1.8/setup.py` & `awsfile-helper-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock', 'boto3']
 
 setup_kwargs = {
     'name': 'awsfile-helper',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'AWS File Helper for Easier I/O',
     'long_description': '# AWS File Helper (awsfile-helper)\nContent Management and Retrieval for Cloud and Local Storage\n\n## Code Usage (Authorization)\nYou must have an AWS Access Key and Secret Access key to connect to AWS.\n\nUpon obtaining these keys, use\n```python\nfrom baseblock import CryptoBase\n\nos.environ[\'AWS_ACCESS_KEY\'] = CryptoBase().encrypt_str(\'<my-access-key>\')\nos.environ[\'AWS_SECRET_KEY\'] = CryptoBase().encrypt_str(\'<my-secret-key>\')\n```\n\nThis will place your encrypted credentials into the environment.\n\nThe `AwsAPI` class will retrieve and decrypt these credentials to login.\n\n## Code Usage (General)\nThe following code will retrieve any file:\n```python\nfrom awsfile_helper import FindOwlFile\n\nd_cloud_file = FindS3File(\n    file_name=\'config/graphviz/stylesheets/nlu\',\n    file_ext=\'yaml\', file_version=\'0.1.0\').process()\n```\nThe bucket is assumed to be `data-core-bast`.\n\nWe can modify this assumption down the road if we create new buckets for different clients, etc.\n\nA file may also be retrieved without a version, like this:\n```python\nd_cloud_file = FindS3File(\n    file_name=\'config/graphviz/stylesheets/nlu\',\n    file_ext=\'yaml\').process()\n```\n\nIn that case, the system will first look in the environment, using a key configuration that relies on the `file_name` like this: `CONFIG_GRAPHVIZ_STYLESHEETS_NLU_VERSION`.  If no value is found in the environment, the system will consider this a _wildcard_ match and set the version to `*`.  This forces the system to list the contents of the qualified path and choose the latest version.  This operation takes an additional 2-3 milliseconds, assuming the network is running smoothly.\n\n\n## Code Usage (Ontologies)\nOntologies require a special finder class, because we typically have two files we want to retrieve - an OWL model and a TXT file with synonyms.\n\nTherefore, assume that an S3 bucket exists with two files we want to retrieve: `syllabus.owl` and `syllabus.txt`.\n\nThe following code will retrieve these files:\n```python\nfrom awsfile_helper import FindOwlFile\n\nd_cloud_file = FindOwlFile(file_name=\'syllabus\', version=\'0.1.0\').process()\n```\n\nNote that we did not specify the file extension within the `file_name` variable.\n\nIt is permissible to specify explicit file names such as `syllabus.txt` or partial file names such.\n\nThe result dictionary is keyed by file name and (with redacted contents) looks like this:\n```json\n{\n    "owl": {\n        "path": "<local path to OWL file">,\n        "version": "<version of OWL file>",\n        "contents": "<contents of OWL file>"\n    },\n    "txt": {\n        "path": "<local path to txt file">,\n        "version": "<version of txt file>",\n        "contents": "<contents of txt file>"\n    }\n}\n```\n',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/awsfile-helper',
```

### Comparing `awsfile-helper-0.1.8/PKG-INFO` & `awsfile-helper-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsfile-helper
-Version: 0.1.8
+Version: 0.1.9
 Summary: AWS File Helper for Easier I/O
 Home-page: https://github.com/craigtrim/awsfile-helper
 License: None
 Keywords: aws,cloud,s3,bucket,helper,utility
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
```

