# Comparing `tmp/odin_sdk_python_check-0.0.2.tar.gz` & `tmp/odin_sdk_python_check-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin_sdk_python_check-0.0.2.tar", max compression
+gzip compressed data, was "odin_sdk_python_check-0.0.3.tar", max compression
```

## Comparing `odin_sdk_python_check-0.0.2.tar` & `odin_sdk_python_check-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1349 2023-07-26 13:53:30.890181 odin_sdk_python_check-0.0.2/README.md
--rw-r--r--   0        0        0     1037 2023-07-26 13:53:30.890344 odin_sdk_python_check-0.0.2/odin/__init__.py
--rw-r--r--   0        0        0     3149 2023-07-26 14:12:22.614416 odin_sdk_python_check-0.0.2/odin/example.py
--rw-r--r--   0        0        0      483 2023-07-26 13:53:30.890521 odin_sdk_python_check-0.0.2/odin/exceptions.py
--rw-r--r--   0        0        0      845 2023-07-26 13:53:30.890656 odin_sdk_python_check-0.0.2/odin/models/__init__.py
--rw-r--r--   0        0        0     1084 2023-07-26 13:56:51.323417 odin_sdk_python_check-0.0.2/odin/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7130 2023-07-26 13:56:51.324923 odin_sdk_python_check-0.0.2/odin/models/__pycache__/certificate_search_response_model.cpython-311.pyc
--rw-r--r--   0        0        0     1558 2023-07-26 13:56:51.325806 odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_certificate_count.cpython-311.pyc
--rw-r--r--   0        0        0    17982 2023-07-26 13:56:51.327761 odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_certificate_hash_details.cpython-311.pyc
--rw-r--r--   0        0        0     2846 2023-07-26 13:56:51.328584 odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_certificates_summary.cpython-311.pyc
--rw-r--r--   0        0        0     1537 2023-07-26 13:56:51.329184 odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_host_count.cpython-311.pyc
--rw-r--r--   0        0        0    15175 2023-07-26 13:56:51.330643 odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_hosts_ip_details_response.cpython-311.pyc
--rw-r--r--   0        0        0     2808 2023-07-26 13:56:51.331459 odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_hosts_summary_response.cpython-311.pyc
--rw-r--r--   0        0        0    16709 2023-07-26 13:56:51.333212 odin_sdk_python_check-0.0.2/odin/models/__pycache__/search_hosts_response_model.cpython-311.pyc
--rw-r--r--   0        0        0     2823 2023-07-26 13:53:30.890779 odin_sdk_python_check-0.0.2/odin/models/certificate_search_response_model.py
--rw-r--r--   0        0        0      434 2023-07-26 13:53:30.890872 odin_sdk_python_check-0.0.2/odin/models/get_certificate_count.py
--rw-r--r--   0        0        0     7214 2023-07-26 13:53:30.890963 odin_sdk_python_check-0.0.2/odin/models/get_certificate_hash_details.py
--rw-r--r--   0        0        0      960 2023-07-26 13:53:30.891046 odin_sdk_python_check-0.0.2/odin/models/get_certificates_summary.py
--rw-r--r--   0        0        0      429 2023-07-26 13:53:30.891141 odin_sdk_python_check-0.0.2/odin/models/get_host_count.py
--rw-r--r--   0        0        0     6693 2023-07-26 13:53:30.891250 odin_sdk_python_check-0.0.2/odin/models/get_hosts_ip_details_response.py
--rw-r--r--   0        0        0      941 2023-07-26 13:53:30.891328 odin_sdk_python_check-0.0.2/odin/models/get_hosts_summary_response.py
--rw-r--r--   0        0        0     7419 2023-07-26 13:53:30.891408 odin_sdk_python_check-0.0.2/odin/models/search_hosts_response_model.py
--rw-r--r--   0        0        0     6154 2023-07-26 14:11:44.622404 odin_sdk_python_check-0.0.2/odin/odin_client.py
--rw-r--r--   0        0        0      459 2023-07-26 14:12:42.769405 odin_sdk_python_check-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 odin_sdk_python_check-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1349 2023-07-26 13:53:30.890181 odin_sdk_python_check-0.0.3/README.md
+-rw-r--r--   0        0        0     1102 2023-07-26 14:17:42.509961 odin_sdk_python_check-0.0.3/odin/__init__.py
+-rw-r--r--   0        0        0     3644 2023-07-26 14:18:24.182195 odin_sdk_python_check-0.0.3/odin/example.py
+-rw-r--r--   0        0        0      483 2023-07-26 13:53:30.890521 odin_sdk_python_check-0.0.3/odin/exceptions.py
+-rw-r--r--   0        0        0      910 2023-07-26 14:18:50.414058 odin_sdk_python_check-0.0.3/odin/models/__init__.py
+-rw-r--r--   0        0        0     1084 2023-07-26 13:56:51.323417 odin_sdk_python_check-0.0.3/odin/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7130 2023-07-26 13:56:51.324923 odin_sdk_python_check-0.0.3/odin/models/__pycache__/certificate_search_response_model.cpython-311.pyc
+-rw-r--r--   0        0        0     1558 2023-07-26 13:56:51.325806 odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_certificate_count.cpython-311.pyc
+-rw-r--r--   0        0        0    17982 2023-07-26 13:56:51.327761 odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_certificate_hash_details.cpython-311.pyc
+-rw-r--r--   0        0        0     2846 2023-07-26 13:56:51.328584 odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_certificates_summary.cpython-311.pyc
+-rw-r--r--   0        0        0     1537 2023-07-26 13:56:51.329184 odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_host_count.cpython-311.pyc
+-rw-r--r--   0        0        0    15175 2023-07-26 13:56:51.330643 odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_hosts_ip_details_response.cpython-311.pyc
+-rw-r--r--   0        0        0     2808 2023-07-26 13:56:51.331459 odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_hosts_summary_response.cpython-311.pyc
+-rw-r--r--   0        0        0    16709 2023-07-26 13:56:51.333212 odin_sdk_python_check-0.0.3/odin/models/__pycache__/search_hosts_response_model.cpython-311.pyc
+-rw-r--r--   0        0        0     2823 2023-07-26 13:53:30.890779 odin_sdk_python_check-0.0.3/odin/models/certificate_search_response_model.py
+-rw-r--r--   0        0        0      434 2023-07-26 13:53:30.890872 odin_sdk_python_check-0.0.3/odin/models/get_certificate_count.py
+-rw-r--r--   0        0        0     7214 2023-07-26 13:53:30.890963 odin_sdk_python_check-0.0.3/odin/models/get_certificate_hash_details.py
+-rw-r--r--   0        0        0      960 2023-07-26 13:53:30.891046 odin_sdk_python_check-0.0.3/odin/models/get_certificates_summary.py
+-rw-r--r--   0        0        0      429 2023-07-26 13:53:30.891141 odin_sdk_python_check-0.0.3/odin/models/get_host_count.py
+-rw-r--r--   0        0        0     1166 2023-07-26 14:20:12.991631 odin_sdk_python_check-0.0.3/odin/models/get_hosts_cve_details.py
+-rw-r--r--   0        0        0     6693 2023-07-26 13:53:30.891250 odin_sdk_python_check-0.0.3/odin/models/get_hosts_ip_details_response.py
+-rw-r--r--   0        0        0      941 2023-07-26 13:53:30.891328 odin_sdk_python_check-0.0.3/odin/models/get_hosts_summary_response.py
+-rw-r--r--   0        0        0     7419 2023-07-26 13:53:30.891408 odin_sdk_python_check-0.0.3/odin/models/search_hosts_response_model.py
+-rw-r--r--   0        0        0     6242 2023-07-26 14:17:09.384373 odin_sdk_python_check-0.0.3/odin/odin_client.py
+-rw-r--r--   0        0        0      459 2023-07-26 14:21:15.407660 odin_sdk_python_check-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 odin_sdk_python_check-0.0.3/PKG-INFO
```

### Comparing `odin_sdk_python_check-0.0.2/README.md` & `odin_sdk_python_check-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/__init__.py` & `odin_sdk_python_check-0.0.3/odin/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,12 @@
-from __future__ import absolute_import
-
-from odin.odin_client import OdinClient
-from odin.exceptions import APIException
 from odin.models.certificate_search_response_model import CertificateSearchResponse
-from odin.models.get_host_count import GetHostsCountResponse
-from odin.models.get_hosts_ip_details_response import GetHostsIpDetailsResponse
-from odin.models.search_hosts_response_model import SearchHostsResponse
-from odin.models.get_hosts_summary_response import GetHostSummaryResponse
 from odin.models.get_certificate_count import GetCertificatesCountResponse
 from odin.models.get_certificate_hash_details import GetCertificateHashDetails
 from odin.models.get_certificates_summary import GetCertificatesSummaryResponse
+from odin.models.get_host_count import GetHostsCountResponse
+from odin.models.get_hosts_cve_details import CVEDetailsResponse
+from odin.models.get_hosts_ip_details_response import GetHostsIpDetailsResponse
+from odin.models.get_hosts_summary_response import GetHostSummaryResponse
+from odin.models.search_hosts_response_model import SearchHostsResponse
 
 
-__all__ = [
-    'OdinClient',
-    'APIException'
-    'CertificateSearchResponse',
-    'GetHostsCountResponse',
-    'GetHostsIpDetailsResponse',
-    'SearchHostsResponse',
-    'GetHostSummaryResponse',
-    'GetCertificatesCountResponse',
-    'GetCertificateHashDetails',
-    'GetCertificatesSummaryResponse',
-]
+__all__ = ['CertificateSearchResponse', 'GetCertificatesCountResponse', 'GetCertificateHashDetails', 'GetCertificatesSummaryResponse', 'GetHostsCountResponse', 'GetHostsIpDetailsResponse', 'GetHostSummaryResponse', 'SearchHostsResponse' ]
```

### Comparing `odin_sdk_python_check-0.0.2/odin/example.py` & `odin_sdk_python_check-0.0.3/odin/example.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,14 @@
         print(response.success)
         print(response.data.count)
         
     except APIException as e:
         print(e.status_code)
         print(e.message)
 
-
-        
 # Example for using get_hosts_ip_details
 def ex_hosts_ip_details():
     try:
         response = client.get_hosts_ip_details("223.217.65.218")
         print(response.success)
         for svc in response.data.services:
             print(f"Service Name: {svc.name}, Port: {svc.port}")
@@ -40,14 +38,25 @@
             start = response.pagination.last
 
         print(response.success)
         print((len(hosts)))
     except APIException as e:
         print(e.status_code)
         print(e.message)
+        
+def ex_hosts_cve_details():
+    # Example for using get_hosts_cve_details
+    try:
+        response = client.get_hosts_cve_details("100.26.248.109")
+        print(response.success)
+        # for cve in response.data:
+        #     print(f"Id: {cve}, Summary: {cve}")
+    except APIException as e:
+        print(e.status_code)
+        print(e.message)
 
 # Example for using get_hosts_summary
 def ex_hosts_summary():
     try:
         response = client.get_hosts_summary("services.port",9)
         for bucket in response.data.buckets:
             print(f"Service: {bucket.key}, Count: {bucket.doc_count}")
@@ -97,8 +106,13 @@
         response = client.get_certificates_summary("certificate.issuer.common_name", 1)
         print(response.success)
         print((len(response.data.buckets)))
     except APIException as e:
         print(e.status_code)
         print(e.message)
 
-client.get_hosts_cve_details()
+if __name__ == "__main__":
+    ex_hosts_count()
+    # ex_certificate_count()
+    # ex_certificate_hash_details()
+    # ex_certificates_summary()
+    # ex_search_certificates()
```

### Comparing `odin_sdk_python_check-0.0.2/odin/models/__pycache__/__init__.cpython-311.pyc` & `odin_sdk_python_check-0.0.3/odin/models/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/__pycache__/certificate_search_response_model.cpython-311.pyc` & `odin_sdk_python_check-0.0.3/odin/models/__pycache__/certificate_search_response_model.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_certificate_count.cpython-311.pyc` & `odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_certificate_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_certificate_hash_details.cpython-311.pyc` & `odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_certificate_hash_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_certificates_summary.cpython-311.pyc` & `odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_certificates_summary.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_host_count.cpython-311.pyc` & `odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_host_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_hosts_ip_details_response.cpython-311.pyc` & `odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_hosts_ip_details_response.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/__pycache__/get_hosts_summary_response.cpython-311.pyc` & `odin_sdk_python_check-0.0.3/odin/models/__pycache__/get_hosts_summary_response.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/__pycache__/search_hosts_response_model.cpython-311.pyc` & `odin_sdk_python_check-0.0.3/odin/models/__pycache__/search_hosts_response_model.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/certificate_search_response_model.py` & `odin_sdk_python_check-0.0.3/odin/models/certificate_search_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/get_certificate_hash_details.py` & `odin_sdk_python_check-0.0.3/odin/models/get_certificate_hash_details.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/get_certificates_summary.py` & `odin_sdk_python_check-0.0.3/odin/models/get_certificates_summary.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/get_hosts_ip_details_response.py` & `odin_sdk_python_check-0.0.3/odin/models/get_hosts_ip_details_response.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/get_hosts_summary_response.py` & `odin_sdk_python_check-0.0.3/odin/models/get_hosts_summary_response.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/models/search_hosts_response_model.py` & `odin_sdk_python_check-0.0.3/odin/models/search_hosts_response_model.py`

 * *Files identical despite different names*

### Comparing `odin_sdk_python_check-0.0.2/odin/odin_client.py` & `odin_sdk_python_check-0.0.3/odin/odin_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 from odin.models.certificate_search_response_model import CertificateSearchResponse
 from odin.models.get_host_count import GetHostsCountResponse
 from odin.models.get_hosts_ip_details_response import GetHostsIpDetailsResponse
 from odin.models.search_hosts_response_model import SearchHostsResponse
 from odin.models.get_hosts_summary_response import GetHostSummaryResponse
+from odin.models.get_hosts_cve_details import CVEDetailsResponse
 from odin.models.get_certificate_count import GetCertificatesCountResponse
 from odin.models.get_certificate_hash_details import GetCertificateHashDetails
 from odin.models.get_certificates_summary import GetCertificatesSummaryResponse
 from odin.exceptions import APIException
 import json
 
 class OdinClient:
@@ -42,15 +43,15 @@
         response = self.make_request(url, req, "POST")
         return GetHostsCountResponse(response)
     
     def get_hosts_cve_details(self, query):
          endpoint = "/hosts/cve/"
          url = self.base_url + endpoint + query
          response = self.make_request(url, None, "GET")
-         return "Hey"
+         return CVEDetailsResponse(response)
                   
     def get_hosts_ip_details(self, query):
         """
         Fetch the latest ip details
         Returns the complete ip details
         return: GetHostsIpDetailsResponse
         """
```

### Comparing `odin_sdk_python_check-0.0.2/PKG-INFO` & `odin_sdk_python_check-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odin-sdk-python-check
-Version: 0.0.2
+Version: 0.0.3
 Summary: Allows to interact easily with the Odin API and access various cybersecurity services, certificate information, and more.
 Author: Anukul Kumar
 Author-email: anukul.kumar@cyble.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

