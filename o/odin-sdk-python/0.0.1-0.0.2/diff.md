# Comparing `tmp/odin_sdk_python-0.0.1.tar.gz` & `tmp/odin_sdk_python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin_sdk_python-0.0.1.tar", max compression
+gzip compressed data, was "odin_sdk_python-0.0.2.tar", max compression
```

## Comparing `odin_sdk_python-0.0.1.tar` & `odin_sdk_python-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,25 @@
--rw-r--r--   0        0        0     1342 2023-07-26 06:24:15.965310 odin_sdk_python-0.0.1/README.md
--rw-r--r--   0        0        0     1037 2023-07-25 14:24:44.149795 odin_sdk_python-0.0.1/odin/__init__.py
--rw-r--r--   0        0        0     3253 2023-07-25 12:33:22.352466 odin_sdk_python-0.0.1/odin/example.py
--rw-r--r--   0        0        0      483 2023-07-24 13:30:01.718847 odin_sdk_python-0.0.1/odin/exceptions.py
--rw-r--r--   0        0        0      845 2023-07-25 11:02:56.332833 odin_sdk_python-0.0.1/odin/models/__init__.py
--rw-r--r--   0        0        0     2823 2023-07-14 03:25:54.374435 odin_sdk_python-0.0.1/odin/models/certificate_search_response_model.py
--rw-r--r--   0        0        0      434 2023-07-12 05:06:57.147103 odin_sdk_python-0.0.1/odin/models/get_certificate_count.py
--rw-r--r--   0        0        0     7214 2023-07-12 05:30:11.746441 odin_sdk_python-0.0.1/odin/models/get_certificate_hash_details.py
--rw-r--r--   0        0        0      960 2023-07-12 05:30:16.127850 odin_sdk_python-0.0.1/odin/models/get_certificates_summary.py
--rw-r--r--   0        0        0      429 2023-07-12 04:48:26.964336 odin_sdk_python-0.0.1/odin/models/get_host_count.py
--rw-r--r--   0        0        0     6693 2023-07-12 04:49:22.181362 odin_sdk_python-0.0.1/odin/models/get_hosts_ip_details_response.py
--rw-r--r--   0        0        0      941 2023-07-12 05:04:30.079384 odin_sdk_python-0.0.1/odin/models/get_hosts_summary_response.py
--rw-r--r--   0        0        0     7419 2023-07-14 03:05:42.334035 odin_sdk_python-0.0.1/odin/models/search_hosts_response_model.py
--rw-r--r--   0        0        0     5945 2023-07-25 11:02:44.728376 odin_sdk_python-0.0.1/odin/odin_client.py
--rw-r--r--   0        0        0      453 2023-07-26 06:23:54.201320 odin_sdk_python-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 odin_sdk_python-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1349 2023-07-26 13:53:30.890181 odin_sdk_python-0.0.2/README.md
+-rw-r--r--   0        0        0     1037 2023-07-26 13:53:30.890344 odin_sdk_python-0.0.2/odin/__init__.py
+-rw-r--r--   0        0        0     3302 2023-07-26 13:59:41.155428 odin_sdk_python-0.0.2/odin/example.py
+-rw-r--r--   0        0        0      483 2023-07-26 13:53:30.890521 odin_sdk_python-0.0.2/odin/exceptions.py
+-rw-r--r--   0        0        0      845 2023-07-26 13:53:30.890656 odin_sdk_python-0.0.2/odin/models/__init__.py
+-rw-r--r--   0        0        0     1084 2023-07-26 13:56:51.323417 odin_sdk_python-0.0.2/odin/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7130 2023-07-26 13:56:51.324923 odin_sdk_python-0.0.2/odin/models/__pycache__/certificate_search_response_model.cpython-311.pyc
+-rw-r--r--   0        0        0     1558 2023-07-26 13:56:51.325806 odin_sdk_python-0.0.2/odin/models/__pycache__/get_certificate_count.cpython-311.pyc
+-rw-r--r--   0        0        0    17982 2023-07-26 13:56:51.327761 odin_sdk_python-0.0.2/odin/models/__pycache__/get_certificate_hash_details.cpython-311.pyc
+-rw-r--r--   0        0        0     2846 2023-07-26 13:56:51.328584 odin_sdk_python-0.0.2/odin/models/__pycache__/get_certificates_summary.cpython-311.pyc
+-rw-r--r--   0        0        0     1537 2023-07-26 13:56:51.329184 odin_sdk_python-0.0.2/odin/models/__pycache__/get_host_count.cpython-311.pyc
+-rw-r--r--   0        0        0    15175 2023-07-26 13:56:51.330643 odin_sdk_python-0.0.2/odin/models/__pycache__/get_hosts_ip_details_response.cpython-311.pyc
+-rw-r--r--   0        0        0     2808 2023-07-26 13:56:51.331459 odin_sdk_python-0.0.2/odin/models/__pycache__/get_hosts_summary_response.cpython-311.pyc
+-rw-r--r--   0        0        0    16709 2023-07-26 13:56:51.333212 odin_sdk_python-0.0.2/odin/models/__pycache__/search_hosts_response_model.cpython-311.pyc
+-rw-r--r--   0        0        0     2823 2023-07-26 13:53:30.890779 odin_sdk_python-0.0.2/odin/models/certificate_search_response_model.py
+-rw-r--r--   0        0        0      434 2023-07-26 13:53:30.890872 odin_sdk_python-0.0.2/odin/models/get_certificate_count.py
+-rw-r--r--   0        0        0     7214 2023-07-26 13:53:30.890963 odin_sdk_python-0.0.2/odin/models/get_certificate_hash_details.py
+-rw-r--r--   0        0        0      960 2023-07-26 13:53:30.891046 odin_sdk_python-0.0.2/odin/models/get_certificates_summary.py
+-rw-r--r--   0        0        0      429 2023-07-26 13:53:30.891141 odin_sdk_python-0.0.2/odin/models/get_host_count.py
+-rw-r--r--   0        0        0     6693 2023-07-26 13:53:30.891250 odin_sdk_python-0.0.2/odin/models/get_hosts_ip_details_response.py
+-rw-r--r--   0        0        0      941 2023-07-26 13:53:30.891328 odin_sdk_python-0.0.2/odin/models/get_hosts_summary_response.py
+-rw-r--r--   0        0        0     7419 2023-07-26 13:53:30.891408 odin_sdk_python-0.0.2/odin/models/search_hosts_response_model.py
+-rw-r--r--   0        0        0     5989 2023-07-26 13:59:07.918835 odin_sdk_python-0.0.2/odin/odin_client.py
+-rw-r--r--   0        0        0      453 2023-07-26 14:05:29.712437 odin_sdk_python-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 odin_sdk_python-0.0.2/PKG-INFO
```

### Comparing `odin_sdk_python-0.0.1/README.md` & `odin_sdk_python-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ```bash
 pip install odin-sdk-python
 ```
 
 ## Examples
 
-In the "example.py", you can find various usage examples demonstrating how to interact with the Odin API using the `odin-sdk` package.
+In the "example.py", you can find various usage examples demonstrating how to interact with the Odin API using the `odin-sdk-python` package.
 
 Each example is a standalone Go program that showcases specific functionalities of the SDK.
 
 ```python
 from odin import OdinClient
 
 client = OdinClient("https://api.getodin.com/v1", "<APIKey>")
```

### Comparing `odin_sdk_python-0.0.1/odin/__init__.py` & `odin_sdk_python-0.0.2/odin/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.1/odin/example.py` & `odin_sdk_python-0.0.2/odin/example.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,19 @@
         response = client.get_hosts_count("string")
         print(response.success)
         print(response.data.count)
         
     except APIException as e:
         print(e.status_code)
         print(e.message)
+
+def test():
+    print("hey")
+    client.test()
+
         
 # Example for using get_hosts_ip_details
 def ex_hosts_ip_details():
     try:
         response = client.get_hosts_ip_details("223.217.65.218")
         print(response.success)
         for svc in response.data.services:
```

### Comparing `odin_sdk_python-0.0.1/odin/models/__init__.py` & `odin_sdk_python-0.0.2/odin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.1/odin/models/certificate_search_response_model.py` & `odin_sdk_python-0.0.2/odin/models/certificate_search_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.1/odin/models/get_certificate_hash_details.py` & `odin_sdk_python-0.0.2/odin/models/get_certificate_hash_details.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.1/odin/models/get_certificates_summary.py` & `odin_sdk_python-0.0.2/odin/models/get_certificates_summary.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.1/odin/models/get_hosts_ip_details_response.py` & `odin_sdk_python-0.0.2/odin/models/get_hosts_ip_details_response.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.1/odin/models/get_hosts_summary_response.py` & `odin_sdk_python-0.0.2/odin/models/get_hosts_summary_response.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.1/odin/models/search_hosts_response_model.py` & `odin_sdk_python-0.0.2/odin/models/search_hosts_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python-0.0.1/odin/odin_client.py` & `odin_sdk_python-0.0.2/odin/odin_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,17 @@
         req = {
             "query": query
         }
         endpoint = "/hosts/count" 
         url = self.base_url + endpoint
         response = self.make_request(url, req, "POST")
         return GetHostsCountResponse(response)
+    
+    def test():
+        print("hey 2")
                   
     def get_hosts_ip_details(self, query):
         """
         Fetch the latest ip details
         Returns the complete ip details
         return: GetHostsIpDetailsResponse
         """
```

### Comparing `odin_sdk_python-0.0.1/PKG-INFO` & `odin_sdk_python-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odin-sdk-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: Allows to interact easily with the Odin API and access various cybersecurity services, certificate information, and more.
 Author: Anukul Kumar
 Author-email: anukul.kumar@cyble.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,15 +22,15 @@
 
 ```bash
 pip install odin-sdk-python
 ```
 
 ## Examples
 
-In the "example.py", you can find various usage examples demonstrating how to interact with the Odin API using the `odin-sdk` package.
+In the "example.py", you can find various usage examples demonstrating how to interact with the Odin API using the `odin-sdk-python` package.
 
 Each example is a standalone Go program that showcases specific functionalities of the SDK.
 
 ```python
 from odin import OdinClient
 
 client = OdinClient("https://api.getodin.com/v1", "<APIKey>")
```

