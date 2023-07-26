# Comparing `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102.tar.gz` & `tmp/echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102.tar", last modified: Mon Jul 24 17:21:54 2023, max compression
+gzip compressed data, was "echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718.tar", last modified: Wed Jul 26 18:48:14 2023, max compression
```

## Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102.tar` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:21:54.963644 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-24 17:20:58.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-24 17:21:54.963644 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-24 17:20:58.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 17:21:54.963644 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-07-24 17:21:52.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:21:54.959644 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:21:54.963644 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 17:20:58.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-24 17:20:58.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    24212 2023-07-24 17:20:58.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1805 2023-07-24 17:20:58.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3520 2023-07-24 17:20:58.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-07-24 17:20:58.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-24 17:20:58.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 17:21:54.963644 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2588 2023-07-24 17:21:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      948 2023-07-24 17:21:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 17:21:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-24 17:21:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-24 17:21:54.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:48:14.325727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 18:48:14.325727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 18:48:14.325727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-07-26 18:48:11.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:48:14.321727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:48:14.321727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    24145 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-26 18:47:13.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:48:14.325727 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-07-26 18:48:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      948 2023-07-26 18:48:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 18:48:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-26 18:48:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-26 18:48:14.000000 echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/LICENSE` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230724172102
+Version: 1.0.0.dev20230726184718
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/README.md` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/setup.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-resample-and-write-to-zarr-store-lambda",
-  version="1.0.0.dev20230724172102",
+  version="1.0.0.dev20230726184718",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,24 @@
     ############################################################################
     def __init__(
             self,
             s3_operations,
             s3fs_operations,
             dynamo_operations,
             sns_operations,
-            input_bucket,
             output_bucket,
             table_name,
             output_bucket_access_key,
             output_bucket_secret_access_key,
             done_topic_arn,
     ):
         self.__s3 = s3_operations
         self.__s3fs = s3fs_operations
         self.__dynamo = dynamo_operations
         self.__sns_operations = sns_operations
-        self.__input_bucket = input_bucket
         self.__output_bucket = output_bucket
         self.__table_name = table_name
         self.__output_bucket_access_key = output_bucket_access_key
         self.__output_bucket_secret_access_key = output_bucket_secret_access_key
         self.__done_topic_arn = done_topic_arn
 
     ############################################################################
@@ -331,15 +329,15 @@
         # )
         # store = s3fs.S3Map(root=s3_zarr_store_path, s3=s3_fs, check=True)
         ### UPDATE 1 ###
         # s3_fs = self.__s3fs(
         #     key=os.getenv('ACCESS_KEY_ID'),  # optional parameter
         #     secret=os.getenv('SECRET_ACCESS_KEY'),
         # )
-        # store = s3fs.S3Map(root=f's3://{self.__input_bucket}/{zarr_path}', s3=s3_fs, check=True)
+        # store = s3fs.S3Map(root=f's3://{self.__output_bucket}/{zarr_path}', s3=s3_fs, check=True)
         ### UPDATE 2 ###
         store = self.__s3fs.s3_map(
             s3_zarr_store_path=zarr_path,
             access_key_id=self.__output_bucket_access_key,
             secret_access_key=self.__output_bucket_secret_access_key
         )
         # You are already using dask, this is assumed by open_zarr, not the same as open_dataset(engine=“zarr”)
@@ -431,15 +429,15 @@
         :return: (list, list, list): Returns the latitude, longitude, and epoch seconds
         needed to properly index the data.
         """
         s3 = s3fs.S3FileSystem(
             key=os.getenv('ACCESS_KEY_ID'),  # optional parameter
             secret=os.getenv('SECRET_ACCESS_KEY'),
         )
-        geo_json_s3_path = f's3://{self.__input_bucket}/{input_zarr_path}/geo.json'
+        geo_json_s3_path = f's3://{self.__output_bucket}/{input_zarr_path}/geo.json'
         assert(s3.exists(geo_json_s3_path)), "S3 GeoJSON file does not exist."
         geo_json = geopandas.read_file(
             filename=geo_json_s3_path,
             storage_options={
                 "key": os.getenv('ACCESS_KEY_ID'),  # Optional values
                 "secret": os.getenv('SECRET_ACCESS_KEY'),
             },
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/lambda_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 from .lambda_executor import LambdaExecutor
 from .s3_operations import S3Operations
 from .s3fs_operations import S3FSOperations
 from .dynamo_operations import DynamoOperations
 from .sns_operations import SnsOperations
 
 
-input_bucket = os.environ['INPUT_BUCKET']
-output_bucket = os.environ['OUTPUT_BUCKET']
 table_name = os.environ['TABLE_NAME']
+# input_bucket = os.environ['INPUT_BUCKET']
+output_bucket = os.environ['OUTPUT_BUCKET']
 output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
 output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
 done_topic_arn = os.environ['TOPIC_ARN']
 
 executor = LambdaExecutor(
     s3_operations=S3Operations(),
     s3fs_operations=S3FSOperations(),
     dynamo_operations=DynamoOperations(),
     sns_operations=SnsOperations(),
-    input_bucket=input_bucket,
+    # input_bucket=input_bucket,
     output_bucket=output_bucket,
     table_name=table_name,
     output_bucket_access_key=os.getenv('OUTPUT_BUCKET_ACCESS_KEY'),
     output_bucket_secret_access_key=os.getenv('OUTPUT_BUCKET_SECRET_ACCESS_KEY'),
     done_topic_arn=done_topic_arn
 )
 
 def handler(sns_event, context):
     print(f"table name: {os.environ['TABLE_NAME']}")
-    print(f"input bucket: {os.environ['INPUT_BUCKET']}")
+    # print(f"input bucket: {os.environ['INPUT_BUCKET']}")
     print(f"output bucket: {os.environ['OUTPUT_BUCKET']}")
     if 'OUTPUT_BUCKET_ACCESS_KEY' in os.environ:
         print(os.environ['OUTPUT_BUCKET_ACCESS_KEY'])
     if 'OUTPUT_BUCKET_SECRET_ACCESS_KEY' in os.environ:
         print(os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY'])
     #
     print("Event : " + str(sns_event))
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda/s3fs_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-resample-and-write-to-zarr-store-lambda
-Version: 1.0.0.dev20230724172102
+Version: 1.0.0.dev20230726184718
 Home-page: https://github.com/ci-cmg/echofish-aws-resample-and-write-to-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230724172102/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-resample-and-write-to-zarr-store-lambda-1.0.0.dev20230726184718/src/echofish_aws_resample_and_write_to_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

